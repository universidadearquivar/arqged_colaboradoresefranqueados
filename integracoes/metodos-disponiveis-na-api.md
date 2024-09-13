---
description: >-
  O ArqGED conta com uma lista de métodos disponíveis para uso, na tabela abaixo
  temos o detalhamento de cada um deles.
---

# 🟩 Métodos disponíveis na API

|  Nº | Classe       | Método                                                                                                                                                                                                                                                      | Versão |   Status   |
| :-: | ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----: | :--------: |
| 1.1 | Autenticacao | [POST/api/Autenticacao/Login](metodos-disponiveis-na-api/1.-autenticacao.md#id-1.1-post-api-autenticacao-login)                                                                                                                                             |    1   | Disponível |
| 1.2 | Autenticacao | [POST/api/Autenticacao/RefreshToken](metodos-disponiveis-na-api/1.-autenticacao.md#id-1.2-post-api-autenticacao-refreshtoken)                                                                                                                               |    1   | Disponível |
| 2.1 | Arquivo      | [GET/api/Arquivo/Get](metodos-disponiveis-na-api/2.-arquivo.md#id-2.1-get-api-arquivo-get)                                                                                                                                                                  |    1   | Disponível |
| 2.2 | Arquivo      | [POST/api/Arquivo/Post](metodos-disponiveis-na-api/2.-arquivo.md#id-2.2-post-api-arquivo-post)                                                                                                                                                              |    1   | Disponível |
| 2.3 | Arquivo      | [POST/api/Arquivo/Upload](metodos-disponiveis-na-api/2.-arquivo.md#id-2.3-post-api-arquivo-upload)                                                                                                                                                          |    1   | Disponível |
| 2.4 | Arquivo      | [DELETE/api/Arquivo/Delete](metodos-disponiveis-na-api/2.-arquivo.md#id-2.4-delete-api-arquivo-delete)                                                                                                                                                      |    1   | Disponível |
| 2.5 | Arquivo      | [GET/api/Arquivo/{idImagem}/Cliente/{idCliente}](metodos-disponiveis-na-api/2.-arquivo.md#id-2.5-get-api-arquivo-idimagem-cliente-idcliente)                                                                                                                |    1   | Disponível |
| 3.1 | Billing      | [GET/api/Billing/Get](metodos-disponiveis-na-api/3.-billing.md#id-3.1-get-api-billing-get)                                                                                                                                                                  |    1   | Disponível |
| 3.2 | Billing      | [GET/api/Billing/Get/Conta](metodos-disponiveis-na-api/3.-billing.md#id-3.2-get-api-billing-get-conta)                                                                                                                                                      |    1   | Disponível |
| 4.1 | Documento    | [PUT/api/Documento/Put](metodos-disponiveis-na-api/4.-documento.md#id-4.1-put-api-documento-put)                                                                                                                                                            |    1   | Disponível |
| 4.2 | Documento    | [POST/api/Documento/Post](metodos-disponiveis-na-api/4.-documento.md#id-4.2-post-api-documento-post)                                                                                                                                                        |    1   | Disponível |
| 4.3 | Documento    | [GET/api/Documento/Get](metodos-disponiveis-na-api/4.-documento.md#id-4.3-get-api-documento-get)                                                                                                                                                            |    1   | Disponível |
| 4.4 | Documento    | [DELETE/api/Documento/Delete](metodos-disponiveis-na-api/4.-documento.md#id-4.4-delete-api-documento-delete)                                                                                                                                                |    1   | Disponível |
| 5.1 | Lista        | [GET/api/Lista/GetListas](metodos-disponiveis-na-api/5.-lista.md#id-5.1.get-api-lista-getlistas)                                                                                                                                                            |    1   | Disponível |
| 5.2 | Lista        | [GET/api/Lista/GetCamposDaLista](metodos-disponiveis-na-api/5.-lista.md#id-5.2.get-api-lista-getcamposdalista)                                                                                                                                              |    1   | Disponível |
| 5.3 | Lista        | [GET/api/Lista/GetLinhaLista](metodos-disponiveis-na-api/5.-lista.md#id-5.3.get-api-lista-getlinhalista)                                                                                                                                                    |    1   | Disponível |
| 5.4 | Lista        | [PUT/api/Lista/{idLista}/Cliente/{idCliente}/LinhaLista/{idLinhaLista}](metodos-disponiveis-na-api/5.-lista.md#id-5.4.put-api-lista-idlista-cliente-idcliente-linhalista-idlinhalista)                                                                      |    1   | Disponível |
| 5.5 | Lista        | [POST/api/AdicionarItemLista/Post](metodos-disponiveis-na-api/5.-lista.md#id-5.5.post-api-adicionaritemlista-post)                                                                                                                                          |    1   | Disponível |
| 5.6 | Lista        | [POST/api/Lista/RetornaLinhaListasPorCampoValor/{idLista}/{idUnidade}/{idCliente}](metodos-disponiveis-na-api/5.-lista.md#id-5.6.post-api-lista-retornalinhalistasporcampovalor-idlista-idunidade-idcliente)                                                |    1   | Disponível |
| 6.1 | Workflow     | [GET/api/ConfWorkflow/{idCliente}](metodos-disponiveis-na-api/6.-workflow.md#id-6.1.get-api-confworkflow-idcliente)                                                                                                                                         |    1   | Disponível |
| 6.2 | Workflow     | [POST/api/Workflow/Ativar](metodos-disponiveis-na-api/6.-workflow.md#id-6.2.post-api-workflow-ativar)                                                                                                                                                       |    1   | Disponível |
| 6.3 | Workflow     | [PATCH/api/Workflow/Cliente/{idCliente}/associar-documentos](metodos-disponiveis-na-api/6.-workflow.md#id-6.3.patch-api-workflow-cliente-idcliente-associar-documentos)                                                                                     |    1   | Disponível |
| 6.4 | Workflow     | [GET/api/ConfWorkflow/{idConfWorkflow}/Cliente/{idCliente}/fluxos-ativados](metodos-disponiveis-na-api/6.-workflow.md#id-6.4.get-api-confworkflow-idconfworkflow-cliente-idcliente-fluxos-ativados)                                                         |    1   | Disponível |
| 6.5 | Workflow     | [GET/api/Workflow/Cliente/{idCliente}/dados-fluxo](metodos-disponiveis-na-api/6.-workflow.md#id-6.5.get-api-workflow-cliente-idcliente-dados-fluxo)                                                                                                         |    1   | Disponível |
| 6.6 | Workflow     | [GET/api/Workflow/Cliente/{idCliente}/modelo-fluxo](metodos-disponiveis-na-api/6.-workflow.md#id-6.6.get-api-workflow-cliente-idcliente-modelo-fluxo)                                                                                                       |    1   | Disponível |
| 6.7 | Workflow     | [PATCH/api/Workflow/EtapaExecucao/{IdWorkflowEtapaExecucao}/Cliente/{idCliente}/atualizar-dados-formulário](metodos-disponiveis-na-api/6.-workflow.md#id-6.7.patch-api-workflow-etapaexecucao-idworkflowetapaexecucao-cliente-idcliente-atualizar-dados-fo) |    1   | Disponível |
| 7.1 | Nota Fiscal  | [POST/api/NotaFiscal/ImportaNotaFiscal](<metodos-disponiveis-na-api/copy-of-page-1 (1).md#id-7.1.post-api-notafiscal-importanotafiscal>)                                                                                                                    |    1   | Disponível |
| 8.1 | Relatórios   | [GET/api/Relatorios/GetRelatorios](metodos-disponiveis-na-api/8.-relatorios.md#id-8.1.get-api-relatorios-getrelatorios)                                                                                                                                     |    1   | Disponível |
| 8.2 | Relatórios   | [GET/api/Relatorios/GetDadosRelatorios](metodos-disponiveis-na-api/8.-relatorios.md#id-8.2.get-api-relatorios-getdadosrelatorios)                                                                                                                           |    1   | Disponível |
| 9.1 | Usuário      | [POST/api/Usuario/AdicionarUsuario](metodos-disponiveis-na-api/9.-usuario.md#id-9.1.post-api-usuario-adicionarusuario)                                                                                                                                      |    1   | Disponível |
| 9.2 | Usuário      | [PATCH/api/Usuario/{IdUsuario}/AlterarSenhaUsuario](metodos-disponiveis-na-api/9.-usuario.md#id-9.2.patch-api-usuario-idusuario-alterarsenhausuario)                                                                                                        |    1   | Disponível |
| 9.3 | Usuário      | [PATCH/api/Usuario/{IdUsuario}/AlterarStatusUsuario](metodos-disponiveis-na-api/9.-usuario.md#id-9.3.patch-api-usuario-idusuario-alterarstatususuario)                                                                                                      |    1   | Disponível |

***

## Códigos Retorno de Validações

### Code: 200 - OK <a href="#code-200-ok" id="code-200-ok"></a>

Este código é a resposta de status de sucesso que indica que a requisição foi bem-sucedida.

### Code: 201 - Created <a href="#code-201-created" id="code-201-created"></a>

Este código é retornado quando a requisição foi bem-sucedida e um registro é criado com sucesso.

### Code: 400 - Bad Request <a href="#code-400-bad-request" id="code-400-bad-request"></a>

Este erro é retornado quando não for possível interpretar a requisição e/ou o servidor tenta processar a solicitação, mas algum parâmetro da solicitação não é válido, por exemplo, um recurso formatado incorretamente ou uma tentativa de requisição com dados faltantes. As informações sobre a solicitação são fornecidas no corpo da resposta e incluem um código de erro e uma mensagem de erro.

**a- Item obrigatório**

**b- Formato incorreto**

**c- Ids inexistente.**

**d- Algum parâmetro está incorreto ou é inexistente**

### Code: 401 – Unauthorized <a href="#code-401-unauthorized" id="code-401-unauthorized"></a>

Este erro é retornado quando ocorre alguma falha na autorização e/ou os parâmetros de autenticação estão incorretos.

### Code: 404 Not Found <a href="#code-404-not-found" id="code-404-not-found"></a>

Este erro é retornado quando o recurso solicitado ou o _endpoint_ não foi localizado.

### Code: 422 - Unprocessable <a href="#code-422-unprocessable" id="code-422-unprocessable"></a>

Este erro é retornado quando a requisição foi recebida com sucesso, porém contém parâmetros inválidos.

### Code: 500 - Server Error <a href="#code-500-server-error" id="code-500-server-error"></a>

Este erro é retornado quando:

* Ocorre um erro interno no servidor.
* Ocorre uma falha na plataforma ArqGed.
* Formato do parâmetro incorreto.
* Formato do JSON incorreto.
