# 1.6.PATCH/api/v1/processo/{idProcesso}/cancelar-processo

O objetivo deste método é permitir que o usuário cancele o processo de assinatura que esteja em andamento.

Neste método o usuário irá nos enviar o ID do Processo, e nós cancelaremos o processo informado.

## Requisição <a href="#requisicao" id="requisicao"></a>

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2Fcontent.gitbook.com%2Fcontent%2FNkvKZtdmOiilgqExqFNO%2Fblobs%2FHpqIB5o59DbmQKxzzaji%2Fapi15.png&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=47a6fc6&#x26;sv=2" alt=""><figcaption></figcaption></figure>

***

## Retorno <a href="#retorno" id="retorno"></a>

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2Fcontent.gitbook.com%2Fcontent%2FNkvKZtdmOiilgqExqFNO%2Fblobs%2FOvkwkEAYNEyJo7ZTMMtk%2Fapi16.png&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=c4cebcca&#x26;sv=2" alt=""><figcaption></figcaption></figure>

### Detalhamento do Retorno <a href="#detalhamento-do-retorno" id="detalhamento-do-retorno"></a>

**Ref. 01 - Código 200:** Como retorno de sucesso, a aplicação retornará o código 200 juntamente com a mensagem de documento cancelado com sucesso.

**Ref. 02 - Código 400:** _Mensagem de item obrigatório:_ Esta mensagem será exibida no singular ou plural quando um ou mais itens obrigatórios não tiver sido enviado na chamada da API.

**Ref. 03 - Código 400:** _Mensagem de formato incorreto:_ Esta mensagem será exibida no singular ou plural quando um ou mais itens estiverem sido enviados com formato incorreto.

**Ref. 04 - Código 400:** _Mensagem de Ids inexistente:_ Esta mensagem será exibida no singular ou plural quando um ou mais Id enviado não existir.

**Ref. 05 - Código 400:** _Mensagem de documento excluído:_ Esta mensagem será exibida quando o processo em questão tiver sido excluído logicamente.

**Ref. 06 - Código 400:** _Mensagem de parâmetro está incorreto ou é inexistente_: Quando a chamada é feita com algum parâmetro escrito errado ou parâmetro que não existe no método.

**Ref. 07 - Código 422:** _Mensagem validações:_ Estas mensagens serão exibidas quando o usuário informar um com status diferente de Aguardando ou Em processo.

**Ref. 08 - Código 401:** _Mensagem de usuário da API não autorizado:_ AppKey inválida ou não localizada.
