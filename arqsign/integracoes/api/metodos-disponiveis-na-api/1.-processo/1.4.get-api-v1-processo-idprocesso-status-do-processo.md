# 1.4.GET/api/v1/processo/{idProcesso}/status-do-processo

Descrição: Buscar status do processo de assinaturas V1.

## Objetivo do Método <a href="#objetivo-do-metodo" id="objetivo-do-metodo"></a>

Este serviço permite aos Clientes, via API, buscar o status de um processo, **não excluído logicamente.**

## Requisição <a href="#requisicao" id="requisicao"></a>

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252Fm8mJCxE7nrYamF2rlA1o%252Fimage.png%3Falt%3Dmedia%26token%3Db2ebce50-a1f6-40f6-86f9-c5fd40653123&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=d442fe7f&#x26;sv=2" alt=""><figcaption></figcaption></figure>

### Detalhamento do Header e Parameters <a href="#detalhamento-do-header-e-parameters" id="detalhamento-do-header-e-parameters"></a>

**Ref. 01:** “AppKey” é a chave de autorização para se autenticar na API. Esta chave deve ser válida e estar vinculada a uma conta ArqSign ativa.

**Ref. 02:** “idProcesso” - Para se obter o status do processo, deve ser enviado como parâmetro o Id do Processo de assinatura na plataforma ArqSign. Este ID a API devolve como retorno de sucesso, após a chamada do método: [**POST/api/v2/processo/enviar-documento-para-assinar.**](https://manual.arquivar.com/manual-arqsign/administracao/integracoes/api/metodos-disponiveis-na-api/1.-processo/1.1.post-api-v2-processo-enviar-documento-para-assinar)

***

## Validações gerais <a href="#validacoes-gerais" id="validacoes-gerais"></a>

O sistema verifica se a AppKey existe, é válida e o status da conta está ativo.

## **Retorno validações** <a href="#retorno-validacoes" id="retorno-validacoes"></a>

### Erro: 400 - Bad Request <a href="#erro-400-bad-request" id="erro-400-bad-request"></a>

Este erro é retornado quando não for possível interpretar a requisição e/ou o servidor tenta processar a solicitação, mas algum parâmetro da solicitação não é válido, por exemplo, um recurso formatado incorretamente ou uma tentativa de requisição com dados faltantes. As informações sobre a solicitação são fornecidas no corpo da resposta e incluem um código de erro e uma mensagem de erro.

1. **Item obrigatório:** Esta mensagem é exibida no singular ou plural quando um ou mais itens obrigatórios não tiver sido enviado na chamada da API.
2. **Formato incorreto:** Esta mensagem é exibida no singular ou plural quando um ou mais itens estiverem sido enviados com formato incorreto.
3. **Ids inexistente:** Esta mensagem é exibida no singular ou plural quando um ou mais Id enviado não existir.
4. **Documento excluído:** Esta mensagem será exibida quando o documento retornar estive excluído logicamente.
5. **Algum parâmetro está incorreto ou é inexistente:** Esta mensagem é exibida quando a chamada é feita com algum parâmetro escrito errado ou quando é enviado uma informação que não existe no método.

### **Erro: 401 – Unauthorized** <a href="#erro-401-unauthorized" id="erro-401-unauthorized"></a>

Este erro é retornado quando a chave de autenticação da API ArqSign está incorreta ou não foi informada corretamente.

### Erro: 404 - Not Found <a href="#erro-404-not-found" id="erro-404-not-found"></a>

Este erro é retornado quando o recurso solicitado ou o endpoint não foi localizado.

### Erro: 422 - Unprocessable <a href="#erro-422-unprocessable" id="erro-422-unprocessable"></a>

Este erro é retornado quando a requisição foi recebida com sucesso, porém contém parâmetros inválidos.

### Erro: 500 - Server Error <a href="#erro-500-server-error" id="erro-500-server-error"></a>

Este erro é retornado quando:

* Ocorre um erro interno no servidor,
* Ocorre uma falha na plataforma ArqSign,
* Formato do JSON incorreto.

## Retorno de sucesso <a href="#retorno-de-sucesso" id="retorno-de-sucesso"></a>

Status 200 - Success

O sistema deve retornar o status do processo no idioma do usuário remetente (IdResponsável).

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FEPCHRZe5iGji16SrfKem%252Fimage.png%3Falt%3Dmedia%26token%3Dc1b8d911-4e75-4e77-8746-5b4d22ad950d&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=ae6eaf7b&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**nomeProcesso**

O sistema retorna o nome do processo.

**status**

O sistema retorna o status do processo.

**idStatus**

O sistema retorna o id do status do processo.

**expirado**

O sistema retorna se o processo está expirado ou não.

1 = true ou 0 = False

Somente processos com status Aguardando ou Em processo pode ter o parâmetro expirado = true. Ou seja, o cálculo para expiração deve ser executado para processos com status Aguardando ou Em processo.

**Como calcular a data de expiração do documento:**

Se **DataReenvio** estiver vazia, Data de expiração do documento = (**DataEnvio + ExpiracaoDias**).

Se **DataReenvio** não estiver vazia, Data de expiração do documento = (**DataReenvio + ExpiracaoDias**).

Somente será retornardo expirado = true, caso a data de hoje seja > que a data da expiração.

**dataConclusao**

O sistema retorna a data de conclusão caso o processo esteja concluído.

**dataCancelamento**

O sistema retorna a data de cancelamento caso o processo esteja cancelado.

**dataExpiracao**

O sistema retorna a data de expiração somente de processo com status Aguardando ou Em processo.

**Como calcular a data de expiração do documento:**

Se **DataReenvio** estiver vazia, Data de expiração do documento = (**DataEnvio + ExpiracaoDias**).

Se **DataReenvio** não estiver vazia, Data de expiração do documento = (**DataReenvio + ExpiracaoDias**).

### Retorno - Exemplo Body <a href="#retorno-exemplo-body" id="retorno-exemplo-body"></a>

<a class="button secondary">Copiar</a>

```json
{
    "nomeProcesso": "string",
    "status": "string",
    "idStatus": "tinyint",
    "expirado": "bit",
    "dataConclusao": "date",
    "dataCancelamento": "date",
    "dataExpiracao": "date"
}
```
