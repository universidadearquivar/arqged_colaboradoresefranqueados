# 1.5.GET/api/v1/processo/{idprocesso}/dados-signatarios

O objetivo deste método é permitir que o usuário busque os dados dos signatários que possuem ação de assinar eletronicamente em um processo de assinatura.

Neste método o usuário irá nos enviar o ID do Processo, e nós retornaremos um JSON completo com as informações do processo e dos signatários.

## Requisição <a href="#requisicao" id="requisicao"></a>

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2Fcontent.gitbook.com%2Fcontent%2FNkvKZtdmOiilgqExqFNO%2Fblobs%2F8KZo4GCFCBa4qjkDVXJ9%2Fapi11.png&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=bab4565a&#x26;sv=2" alt=""><figcaption></figcaption></figure>

### Detalhamento do Header e Parameters <a href="#detalhamento-do-header-e-parameters" id="detalhamento-do-header-e-parameters"></a>

**Ref. 01:** “AppKey” é a chave de autorização para se autenticar na API. Esta chave deve ser válida e estar vinculada a uma conta ArqSign ativa.

**Ref. 02:** “idProcesso” - Para se obter o status do processo deve ser enviado como parâmetro o ID do processo de assinatura na plataforma ArqSign. Este ID a API devolve como retorno de sucesso, após a chamada do método: [**POST/api/v2/processo/enviar-documento-para-assinar**.](https://manual.arquivar.com/manual-arqsign/administracao/integracoes/api/metodos-disponiveis-na-api/1.-processo/1.1.post-api-v2-processo-enviar-documento-para-assinar)

Outra forma de obter o ID do processo e por meio da plataforma ArqSign, na opção “Histórico” do documento disponível nas caixas de [Entrada](https://manual.arquivar.com/manual-arqsign/caixa-postal/caixa-de-entrada), [Enviados](https://manual.arquivar.com/manual-arqsign/caixa-postal/enviados) e [Excluídos](https://manual.arquivar.com/manual-arqsign/caixa-postal/excluidos).

***

## Validações Gerais <a href="#validacoes-gerais" id="validacoes-gerais"></a>

O sistema deve verificar se a AppKey existe, é válida e a conta está com status ativo.

## Retorno validações <a href="#retorno-validacoes" id="retorno-validacoes"></a>

### Erro: 400 - Bad Request <a href="#erro-400-bad-request" id="erro-400-bad-request"></a>

Este erro é retornado quando não for possível interpretar a requisição e/ou o servidor tenta processar a solicitação, mas algum parâmetro da solicitação não é válido, por exemplo, um recurso formatado incorretamente ou uma tentativa de requisição com dados faltantes. As informações sobre a solicitação são fornecidas no corpo da resposta e incluem um código de erro e uma mensagem de erro.

1. **Item obrigatório:** Esta mensagem é exibida no singular ou plural quando um ou mais itens obrigatórios não tiver sido enviado na chamada da API.
2. **Formato incorreto:** Esta mensagem é exibida no singular ou plural quando um ou mais itens estiverem sido enviados com formato incorreto.
3. **Ids inexistente:** Esta mensagem é exibida no singular ou plural quando um ou mais Id enviado não existir.
4. **Documento excluído:** Esta mensagem será exibida quando o documento retornar estive excluído logicamente.
5. **Algum parâmetro está incorreto ou é inexistente:** Esta mensagem é exibida quando a chamada é feita com algum parâmetro escrito errado ou quando é enviado uma informação que não existe no método.

### Erro: 401 – Unauthorized <a href="#erro-401-unauthorized" id="erro-401-unauthorized"></a>

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

O sistema retorna os dados dos signatários do processo com ação de **Assinar Online**.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252F887LlhJZIyrSMcOuQVN4%252Fimage.png%3Falt%3Dmedia%26token%3Db6adbeb9-43cb-452b-9e18-215639d3c66d&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=1178c485&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**nomeProcesso**

O sistema retorna o nome do processo.

**status**

O sistema retorna o status do processo.

**idStatus**

O sistema retorna o id do status do processo.

**dataConclusao**

O sistema retorna a data de conclusão do processo, se houver

**dataCancelamento**

O sistema retorna a data de cancelamento do processo, se houver

**usuarioCancelamento**

O sistema retorna o nome do usuário quem cancelou o processo, se houver

**dataExpiracao**

O sistema retorna a data de expiração do processo, conforme a configuração e a data de envio/reenvio do documento.

Se **dataReenvio** for igual a null, então **dataExpiracao = dataEnvio + ExpiracaoDias**

Se **dataReenvio** for diferente de null, então **dataExpiracao = dataReenvio + expiracaoDias**

**signatários**

Nesta parte do JSON, o sistema retorna os dados dos signatários do processo.

> **ordem**
>
> O sistema retorna a ordem de assinatura do signatário.

> **idProcessoDestinatario**
>
> O sistema retorna o id do processo destinatário.

> **nome**
>
> O sistema retorna nome do signatário.

> **idTipoAssinatura**
>
> O sistema retorna o tipo de assinatura do signatário.
>
> 1 - Assinatura Eletrônica
>
> 3 - Certificado Digital - ICP Brasil
>
> 4 - Certificado Digital - Outros

> **idFormaEnvioProcesso**
>
> O sistema retorna a forma de envio do processo para o signatário.
>
> 1 - E-mail
>
> 2 - Whatsapp

> **email**
>
> O sistema retorna e-mail do signatário o qual o processo foi enviado.

> **telefone**
>
> O sistema retorna o telefone do signatário para o qual o processo foi enviado.

> **papelSignatario**
>
> 1. **pessoaFisica**
>
> O sistema retorna os papeis do signatário como pessoa física, se houver.
>
> 1. **pessoaJuridica**
>
> O sistema retorna os papeis do signatário como pessoa jurídica, se houver.

> **tipoAcao**
>
> O sistema retorna o tipo de ação do signatário no processo.

> **idTipoAcao**
>
> O sistema retorna o id do tipo de ação do signatário no processo.

> **idMeioEnvioCodigoSeguranca**
>
> O sistema retorna o id do meio de envio do código de segurança, se houver.
>
> 1- SMS (Somente Brasil)
>
> 2 - Whatsapp
>
> 3 - Email
>
> 4 - Não enviar

> **emailSeguranca**
>
> O sistema retorna o email que o código de segurança foi enviado.

> **telefoneSeguranca**
>
> O sistema retorna o telefone que o código de segurança foi enviado.

> **permitirReenviarCodigo**
>
> O sistema retorna a informação se permite o reenvio do código de segurança.
>
> 1 = true ou 0 = False

> **falhaEnvio**
>
> O sistema retorna a informação se houve falha no envio do processo.
>
> 1= true ou 0 = false.

> **falhaEnvioCodigoSeguranca**
>
> O sistema retorna a informação se houve falha no envio do código de segurança.
>
> 1= true ou 0 = false.

> **assinado**
>
> O sistema retorna a informação se o signatário assinou os documentos.
>
> 1 = true ou 0 = False.

> **dataAssinatura**
>
> O sistema retorna a data da assinatura, se houver.

> **assinaturaRecusada**
>
> O sistema retorna a informação se a assinatura foi recusada ou não.
>
> 1= true ou 0 = False

> **motivoRecusa**
>
> O sistema retorna o motivo da recusa, se houver.

> **anexos**
>
> O sistema retorna os dados dos anexos dos signatários, se houver.
>
> 1. **id**
>
> O sistema retorna o id do anexo do signatário. 
>
> 1. **anexoDocumentoNome**
>
> O sistema retorna o **nome do signatários + nome configuração + o nome anexo do signatário (com a extensão).** 

### Exemplo de JSON de Retorno <a href="#exemplo-de-json-de-retorno" id="exemplo-de-json-de-retorno"></a>

**Exemplo Body**

<a class="button secondary">Copiar</a>

```json
{ 
    "nomeProcesso": "string", 
    "status": "string", 
    "idStatus": "tinyint", 
    "dataConclusao": "datetime", 
    "dataCancelamento": "datetime", 
    "usuarioCancelamento": "string", 
    "dataExpiracao": "datetime", 
    "signatarios": [ 
        { 
            "ordem": "tinyint", 
            "IdProcessoDestinatario": "guid", 
            "nome": "string", 
            "idTipoAssinatura": "tinyint", 
            "IdFormaEnvioProcesso": "bit", 
            "email": "string", 
            "telefone": "string", 
            "papelSignatario": { 
                "pessoaFisica": [ 
                    "varchar(50)", 
                    "varchar(50)", 
                    "varchar(50)" 
                ], 
                "pessoaJuridica": [ 
                    "varchar(50)" 
                ] 
            }, 
            "tipoAcao": "string", 
            "idTipoAcao": "tinyint", 
            "IdMeioEnvioCodigoSeguranca": "bit", 
            "emailSeguranca": "string", 
            "telefoneSeguranca": "string", 
            "permitirReenviarCodigo": "bit", 
            "falhaEnvio": "bit", 
            "falhaEnvioCodigoSeguranca": "bit", 
            "assinado": "bit", 
            "dataAssinatura": "datetime"    
            "assinaturaRecusada": "bit", 
            "motivoRecusa": "string",   
            "anexos": [ 
                { 
                    "id": "guid", 
                    "anexoDocumentoNome": "string" 
                } 
            ] 
        } 
    ] 
} 
```
