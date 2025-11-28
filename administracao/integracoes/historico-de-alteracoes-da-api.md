---
icon: rectangle-history
---

# Histórico de alterações da API

## 2025

<details>

<summary>2.19.0 - 02/07/2025</summary>

**V1**

[<mark style="color:blue;">**API de integração:**</mark> <mark style="color:blue;">**Método GET api/v1/processo/{idProcesso}/status-do-processo**</mark>](https://manual.arquivar.com/manual-arqsign/administracao/integracoes/api/metodos-disponiveis-na-api/1.-processo/1.4.get-api-v1-processo-idprocesso-status-do-processo)

Descrição: Buscar status do processo de assinaturas V1.

Objetivo do Método: Este serviço permite aos Clientes, via API, buscar o status de um processo, não excluído logicamente.

Alteração:

* Retornar também o parâmetro `idStatus.`

**V2**

[<mark style="color:blue;">**API de integração: Método GET api/v2/processo/{idProcesso}?arquivoTipo =1\&retornarRegistroAssinatura=true**</mark>](https://manual.arquivar.com/manual-arqsign/administracao/integracoes/api/metodos-disponiveis-na-api/1.-processo/1.2.get-api-v2-processo-idprocesso-arquivotipo-1-and-retornarregistroassinatura-true#objetivo-do-metodo)

Descrição: Buscar informações completas do processo de assinaturas V2 (metadados, signatários e documentos).

Objetivo do Método: Este serviço permite aos Clientes, via API, buscar um processo (não excluído) com todos os seus dados, incluindo signatários e documentos associados.

Alterações:

* Adição do parâmetro `arquivoTipo` (1=Base64, 2=link de download).
* Adição do parâmetro `retornarRegistroAssinatura` (inclui ou não o registro de assinatura).
* Expansão do retorno com novos campos de processo, lembretes, dados completos de signatários e documentos.

**V3**

[<mark style="color:blue;">**API de integração: Método POST /api/v3/processo/enviar-documento-para-assinar**</mark>](https://manual.arquivar.com/manual-arqsign/administracao/integracoes/api/metodos-disponiveis-na-api/1.-processo/1.1.1.post-api-v3-processo-enviar-documento-para-assinar)

Descrição: Enviar processo e documentos para assinatura V3.

Objetivo do Método: Este serviço permite aos Clientes, via API, enviar um ou mais documentos para assinatura, especificando responsáveis e destinatários.

Alteração única em relação à V2:

* Inclusão da opção `linkDocumento` — se informada, o documento será referenciado via link do repositório do cliente e **não** será enviado em Base64; caso **não** seja enviada essa tag, mantém-se o envio em Base64 como na V2.

</details>

<details>

<summary>2.16.0 - 02/06/2025</summary>

O foco desta versão está no retorno de dados dos endpoints abaixo:&#x20;

[**API de integração: Método GET api/v1/processo{idProcesso}/status-do-processo** ](https://manual.arquivar.com/manual-arqsign/administracao/integracoes/api/metodos-disponiveis-na-api/1.-processo/1.4.get-api-v1-processo-idprocesso-status-do-processo)

Descrição: Buscar status do processo de assinaturas V1.&#x20;

Objetivo do Método: Este serviço permite aos Clientes, via API, buscar o status de um processo, não excluído logicamente&#x20;

**Alteração:** retornar também o parâmetro idStatus&#x20;



[**API de integração: Método GET api /v1 /processo /{idProcesso}/dados-signatarios** ](https://manual.arquivar.com/manual-arqsign/administracao/integracoes/api/metodos-disponiveis-na-api/1.-processo/1.5.get-api-v1-processo-idprocesso-dados-signatarios)

Descrição: Buscar dados dos signatários V1.&#x20;

Objetivo do Método: Este serviço permite aos Clientes, via API, buscar os dados dos signatários do processo, não excluído logicamente, com ação de Assinar Online (tipoAcao = 1)&#x20;

Não deve retornar dados dos signatários com ação de Receber Cópia (tipoAcao = 2)&#x20;

**Alteração:** Retornar também os parâmetros&#x20;

"idStatus"&#x20;

"dataConclusao"&#x20;

"dataCancelamento"&#x20;

"usuarioCancelamento"&#x20;

"idTipoAcao"&#x20;

"falhaEnvioCodigoSeguranca"&#x20;

"dataAssinatura"&#x20;

"assinaturaRecusada"&#x20;

"motivoRecusa"&#x20;

"anexos" \["id", "anexoDocumentoNome"]&#x20;

&#x20;

[**API de integração: Método GET api/v2/processo/{idProcesso}"** ](https://manual.arquivar.com/manual-arqsign/administracao/integracoes/api/metodos-disponiveis-na-api/1.-processo/1.2.get-api-v2-processo-idprocesso)

Alteração: Retornar também os parâmetros&#x20;

idStatus&#x20;

idTipoAcao&#x20;

idTipoAssinatura&#x20;

falhaEnvioCodigoSeguranca&#x20;

LinkDocumentoCompartilhado&#x20;

&#x20;

[**API de integração: Método: POST api/v1/conta/buscar-consumo-itens-assinatura**  ](https://manual.arquivar.com/manual-arqsign/administracao/integracoes/api/metodos-disponiveis-na-api/4.-conta/4.2.post-api-v1-conta-buscar-consumo-itens-assinatura)

Descrição: Buscar o uso e consumo dos itens da assinatura da conta V1. &#x20;

Objetivo do Método: Este serviço permite buscar a quantidade do item de envios (Envios, WhatsApp, SMS) que a conta usou em determinado período. &#x20;

**Alteração:** Ajustado o retorno deste endpoint para não contabilizar itens de envios processos cancelados no período consultado.&#x20;

</details>

<details>

<summary>2.15.0 - 20/05/2025</summary>

* Ajuste da API [enviar processo para assinar](https://manual.arquivar.com/manual-arqsign/administracao/integracoes/api/metodos-disponiveis-na-api/1.-processo/1.1.post-api-v2-processo-enviar-documento-para-assinar):

</details>

<details>

<summary>2.8.0 - 30/01/2025</summary>

* Ajuste da API [buscar dados da assinatura da conta](api/metodos-disponiveis-na-api/4.-conta/4.3.get-api-v1-conta-dados-assinatura.md):
  * Alterado o serviço de buscar dados da assinatura da conta para retornar o idStatus da conta 1 - Ativo, 2 - Inativo, 3 - Bloqueado, 4 - Pendente. 
* Melhorias nos parâmetros de retorno do [Webhook](webhook.md).

</details>
