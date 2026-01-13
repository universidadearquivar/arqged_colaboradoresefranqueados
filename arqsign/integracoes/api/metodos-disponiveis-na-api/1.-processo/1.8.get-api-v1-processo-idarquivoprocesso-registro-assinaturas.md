# 1.8.GET/api/v1/processo/{idArquivoProcesso}/registro-assinaturas

Este serviço permite buscar o base64 do registro de assinatura de um arquivo processo.

## Validações <a href="#validacoes" id="validacoes"></a>

### Validações gerais <a href="#validacoes-gerais" id="validacoes-gerais"></a>

1- O usuário deve informar AppKey e SubscriptionKey (SubscriptionKey1 ou SubscriptionKey2) da conta.

2- Somente conta com status Ativo pode permitir buscar o registro de assinatura de um ArquivoProcesso via integração ArqSign.

3- O sistema retorna o registro de assinatura somente para **processos com status diferente de criado.**

## Retorno validações <a href="#retorno-validacoes" id="retorno-validacoes"></a>

### Erro: 400 - Bad Request <a href="#erro-400-bad-request" id="erro-400-bad-request"></a>

Este erro é retornado quando não for possível interpretar a requisição e/ou o servidor tenta processar a solicitação, mas algum parâmetro da solicitação não é válido, por exemplo, um recurso formatado incorretamente ou uma tentativa de requisição com dados faltantes. As informações sobre a solicitação são fornecidas no corpo da resposta e incluem um código de erro e uma mensagem de erro.

**a- Item obrigatório:** Esta mensagem é exibida no singular ou plural quando um ou mais itens obrigatórios não tiver sido enviado na chamada da API.

> **Mensagem:** O(s) item(ns) listado(s) é(são) obrigatório(s): “nome dos itens separados por vírgula”.

**b- Formato incorreto:** Esta mensagem é exibida no singular ou plural quando um ou mais itens estiverem sido enviados com formato incorreto.

> **Mensagem:** O(s) item(ns) listado(s) está(ão) com o formato incorreto: “nome dos itens separados por vírgula”.

**c- Ids inexistente:** Esta mensagem é exibida no singular ou plural quando um ou mais Id enviado não existir.

> **Mensagem:** O(s) id(s) listado(s) não existe(m): “nome dos itens que são Ids de tabela, separados por vírgula”.

**d- Algum parâmetro está incorreto ou é inexistente:** Esta mensagem é exibida quando a chamada é feita com algum parâmetro escrito errado ou quando é enviado uma informação que não existe no método.

> **Mensagem:** Algum parâmetro está incorreto ou é inexistente.

### Erro: 401 – Unauthorized <a href="#erro-401-unauthorized" id="erro-401-unauthorized"></a>

Este erro é retornado quando a chave de autenticação da API ArqSign está incorreta ou não foi informada corretamente.

### Erro: 404 - Not Found <a href="#erro-404-not-found" id="erro-404-not-found"></a>

Este erro é retornado quando o recurso solicitado ou o _endpoint_ não foi localizado.

### Erro: 500 - Server Error <a href="#erro-500-server-error" id="erro-500-server-error"></a>

Este erro é retornado quando:

* Ocorre um erro interno no servidor;
* Ocorre uma falha na plataforma ArqSign;
* Formato do JSON incorreto.

## Retorno de sucesso <a href="#retorno-de-sucesso" id="retorno-de-sucesso"></a>

Status 200 - Success

O sistema retorna o arquivo em formato base64 do registro de assinatura para o idArquivoProcesso informado.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FYdGjTQaJ4xfvx2sw3KFa%252Fimage.png%3Falt%3Dmedia%26token%3Dac8d501f-92c6-403e-aff8-d4aeda328a41&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=d847098d&#x26;sv=2" alt=""><figcaption></figcaption></figure>

#### Dados do registro de assinaturas <a href="#dados-do-registro-de-assinaturas" id="dados-do-registro-de-assinaturas"></a>

**1 - id**

O sistema retorna o id do arquivo processo a que se refere o registro de assinatura.

**2 - nome**

O sistema retorna o nome do documento a que se refere o registro de assinatura + a palavra “Registro de Assinaturas”. Exemplo: “Contrato\_Registro de Assinaturas.pdf”

**3 - base64**

O sistema retorna o base64 do registro de assinatura.

### Retorno - Exemplo Body Response <a href="#retorno-exemplo-body-response" id="retorno-exemplo-body-response"></a>

<a class="button secondary">Copiar</a>

```json
{
  "idArquivoProcesso": "guid",
  "nome": "string",
  "base64": "base64",
}
```
