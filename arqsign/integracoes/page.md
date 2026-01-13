# Fluxo Ideal de Integração

O fluxo ideal de integração ArqSIGN deve combinar o uso da API ArqSIGN + Webhook ArqSIGN.

Desta forma, para a melhor automatização possível, é importante configurar dois Webhooks, um para acompanhamento e outro para conclusão:

## Webhook de Acompanhamento <a href="#webhook-de-acompanhamento" id="webhook-de-acompanhamento"></a>

O objetivo do webhook de acompanhamento é manter o seu sistema atualizado quanto as principais ações relacionadas ao documento além de indicar momentos importantes para se chamar outras APIs ArqSIGN.

Observe abaixo, que no retorno do webhook de acompanhamento sugerimos não incluir nenhum dado de documento, porque enquanto o processo não é concluído, é desnecessário ficar trafegando arquivos que podem ser muito grandes.

### Gatilhos <a href="#gatilhos" id="gatilhos"></a>

* Processo assinado por algum signatário
* Processo com falha de envio
* Processo recusado por algum signatário
* Processo cancelado pelo remetente
* Processo expirado

### Retorno <a href="#retorno" id="retorno"></a>

* Dados do processo
* Signatários

## Webhook de Conclusão <a href="#webhook-de-conclusao" id="webhook-de-conclusao"></a>

O objetivo do webhook de conclusão é enviar ao seu sistema o arquivo assinado por todos os signatários. Neste momento pode ser enviado o Base64 ou o link tanto do arquivo assinado quanto do seu registro de assinatura. O mundo ideal é o webhook enviar ao seu endpoint a URL destes arquivos, e a sua aplicação manipular esta URL para realizar o download. Mas se isso não for possível, o webhook pode ser configurado para enviar o Base64.

### Gatilhos <a href="#gatilhos-1" id="gatilhos-1"></a>

* Processo assinado/concluído por todos os signatários

### Retorno <a href="#retorno-1" id="retorno-1"></a>

* Dados do processo
* Signatários
* Documentos
  * Arquivos do processo: Link para baixar arquivo
  * Link dos documentos compartilhados
  * Registro de assinatura: Link para baixar o arquivo

Com os dois Webhooks acima configurados, será possível implementar o fluxo de integração abaixo.

## Fluxo de Integração <a href="#fluxo-de-integracao" id="fluxo-de-integracao"></a>

<figure><img src="../../.gitbook/assets/image (369).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (370).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (371).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (372).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (373).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (374).png" alt=""><figcaption></figcaption></figure>

### Detalhamento do fluxo <a href="#detalhamento-do-fluxo" id="detalhamento-do-fluxo"></a>

1. **Envio de Documento aos Signatários**

Nesta fase o Cliente deverá implementar a chamada do método POST responsável por enviar o documento a ser assinado na Plataforma ArqSIGN.

**Método:**

> **Nome:** Enviar processo de assinaturas V2.
>
> **URL:** POST [https://api-rest.arqsign.com/api/v2/processo/enviar-documento-para-assinar](https://api-rest.arqsign.com/api/v2/processo/enviar-documento-para-assinar)
>
> **Documentação:** [https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a4640eeaf71857525](https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a4640eeaf71857525)

1. **Acompanhamento: Falha**

Quando houver alguma falha na entrega dos documentos a serem assinados para algum signatário, a aplicação ArqSIGN acionará o Webhook que irá chamar o serviço (URL) do Cliente conforme configurado.

Após este retorno do Webhook o Cliente poderá implementar a chamada do método PATCH responsável por reenviar o processo. Este método pode ser usado para editar a forma de envio para os signatários que tiveram falha na entrega.

**Método:**

> **Nome:** Editar e Reenviar o processo para os destinatários pendentes de assinaturas V2.
>
> **URL:** PATCH [https://api-rest.arqsign.com/api/v2/processo/{idProcesso}/reenviar-processo](https://api-rest.arqsign.com/api/v2/processo/%7BidProcesso%7D/reenviar-processo)
>
> **Documentação:** [https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a21b37c983bbe8bbe](https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a21b37c983bbe8bbe)

1. **Acompanhamento: assinado por algum signatário**

Quando algum signatário assinar o documento, a aplicação ArqSIGN acionará o Webhook que irá chamar o serviço (URL) do Cliente conforme configurado.

O Cliente poderá com os dados retornados pelo Webhook atualizar seu sistema para manter seus dados atualizados.

1. **Acompanhamento: recusa ou cancelamento**

O cancelamento do processo pode ocorrer de três formas:

* Quando algum signatário se recusa a assinar o documento;
* Quando o responsável pelo envio do documento, cancela o processo via aplicação ArqSIGN;
* Quando o cliente chama o método de API PATCH Processo/Cancelar-Processo para cancelar o processo.

Quando o cancelamento ocorrer, o Webhook irá chamar o endpoint do Cliente conforme confirmado com a informação: se o processo foi cancelado ou se algum signatário se recusou a assinar. Quando o signatário se recusa assinar, a aplicação obriga que ele informe uma justificativa, esta justificativa também é enviada pelo Webhook.

A partir deste ponto, o Cliente poderá tratar o retorno e decidir se deve iniciar o processo novamente com a chamada do POST para enviar um novo documento para assinar (Passo 1).

1. **Acompanhamento: Expiração**

Quando o documento expirar, a aplicação ArqSIGN acionará o Webhook que irá chamar o endpoint do Cliente conforme configurado.

Após este retorno do Webhook o Cliente poderá implementar a chamada do método POST responsável por reenviar o processo. Este método irá atualizar o token de assinatura para os signatários que ainda não assinaram o documento.

**Método:**

> **Nome:** Editar e Reenviar o processo para os destinatários pendentes de assinaturas V2.
>
> **URL:** PATCH [https://api-rest.arqsign.com/api/v2/processo/{idProcesso}/reenviar-processo](https://api-rest.arqsign.com/api/v2/processo/%7BidProcesso%7D/reenviar-processo)
>
> **Documentação:** [https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a21b37c983bbe8bbe](https://developers.arqsign.com/api-details#api=api-rest-arqsign\&operation=6734bb1a21b37c983bbe8bbe)

1. **Conclusão**

Quando o último signatário assinar o documento, a aplicação ArqSIGN acionará o Webhook que irá chamar o endpoint do Cliente conforme configurado.

Após este retorno do Webhook o Cliente poderá armazenar em seu sistema o documento assinado juntamente com seu registro de assinatura.

Observe que configurando dois webhooks conforme nossa sugestão, o documento assinado e concluído será trafegado somente neste momento, pelo Webhook de Conclusão.
