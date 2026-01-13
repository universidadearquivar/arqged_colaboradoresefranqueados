---
icon: lightbulb-exclamation-on
---

# Novidades do ArqGED - Histórico

**04/2025**

<details>

<summary>17/04 - Autenticação multifator (MFA)</summary>

**MFA**

O "[**Login com MFA**](https://manual.arquivar.com/manual-arqged-or-interno#login-com-mfa-autenticacao-multifator)" refere-se ao acesso por meio de autenticação multifator. A sigla MFA (do inglês _Multifactor Authentication_) representa um método de segurança que exige que o usuário forneça duas ou mais formas de autenticação para acessar uma aplicação.

Essa abordagem adiciona uma camada extra de proteção, tornando o acesso não autorizado mais difícil, mesmo que a senha do usuário seja comprometida.

<div align="left"><figure><img src="../.gitbook/assets/image (343).png" alt="" width="179"><figcaption></figcaption></figure></div>

**Como funciona no ArqGED**

No ArqGED, o processo de login com MFA funciona da seguinte forma:

**1.** O usuário informa seu **nome de usuário e senha.**

**2.** Em seguida, deverá informar um **código de verificação.**

Esse código é **dinâmico** e muda a cada tentativa de login.

O código pode ser obtido de duas maneiras:

**Via Aplicativo Autenticador** O usuário pode escolher entre diversos aplicativos gratuitos disponíveis no mercado, como:

* Google Authenticator
* Microsoft Authenticator

Para utilizar essa opção, é necessário instalar o aplicativo escolhido no celular e seguir as instruções de configuração no ArqGED.

**Via E-mail** O código de verificação será enviado para o e-mail cadastrado no usuário. Para utilizar essa opção, é preciso validar previamente o e-mail seguindo o fluxo indicado no ArqGED.

**Usuários com acesso via SSO**

Usuários de clientes que utilizam **SSO (Single Sign-On)** para acessar o ArqGED **não utilizarão o MFA do ArqGED**, uma vez que a autenticação com múltiplos fatores estará configurada e gerenciada diretamente pelo SSO do cliente.

</details>

**07/2024**

<details>

<summary>10/07 - Workflow - Copiar dados do fluxo de origem</summary>

**Workflow > Desenho do fluxo**

A tela de configuração para o componente de [“**Novo Fluxo**”](https://arquivar.gitbook.io/manual-arqged-or-colaboradores-e-franqueados/workflow/desenho-do-fluxo/aba-fluxograma#configuracoes-de-fluxo), foi alterada para possibilitar ao usuário copiar os dados do fluxo atual para o novo fluxo.

Anteriormente, no avanço para este componente apenas a aplicação ativava um novo fluxo. Com esta alteração, o usuário poderá configurar previamente, quais informações do fluxo atual poderão ser copiadas para o fluxo de destino.

</details>

**06/2024**

<details>

<summary>17/06 - Ajustes nas permissões</summary>

A aplicação foi alterada para possibilitar ao usuário utilizar as telas do menu Documentos de forma isolada, conforme a necessidade de acesso ou política de segurança da empresa.

As telas do menu Documento, eram exibidas para o usuário por compartilharem as mesmas operações de acesso, como por exemplo: Visualizar documentos, upload de arquivos, excluir documentos e outras de uso em comum para edição/visualização de documentos.

São as telas:

* Cadastrar
* Explorar
* Localização Simples
* Localização Avançada

![](<../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png>)

Com esta mudança, um usuário poderá por exemplo, acessar apenas a tela Cadastrar do menu Documento, sem que haja vínculo ou acesso para as demais telas do mesmo menu.

<mark style="color:green;">**Exemplos de formas de uso a partir do ajuste:**</mark>

* Um usuário poderá acessar apenas a tela **Cadastrar** e, visualizar somente os documentos cadastrados por ele;
* Um usuário poderá acessar apenas a tela **Explorar** e, visualizar/digitalizar documentos sem vínculo com as demais telas do menu;
* Um usuário poderá acessar apenas a tela **Localização Simples** e realizar pesquisas por conteúdo sem vínculo com as demais telas do menu;
* Um usuário poderá acessar apenas a tela **Localização Avançada** e realizar pesquisas sem vínculo com as demais telas do menu.

Além da melhoria para o uso das telas do menu Documentos, houve um impacto importante e significativo para o menu **Workflow**, permitindo que um usuário possa cadastrar um documento no fluxo, sem que ele tenha acesso às telas **Cadastrar** e **pesquisas de documentos** (Explorar, Localização Simples, Localização Avançada).

</details>

**05/2024**

<details>

<summary>30/05 - Componente de Notificação E-mail</summary>

**Workflow > Desenho do Fluxo - Componente de e-mail**

O desenho de fluxo foi alterado para permitir "N" entradas para configuração do componente de e-mail, ou seja, é possível ter várias tarefas terminando neste componente, responsável por enviar notificações do andamento das atividades do fluxo.

Conforme a imagem abaixo, o componente de e-mail recebe 3 avanços de tarefas, sendo permitido "N" entradas e apenas 1 saída para o componente.

![](<../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png>)

</details>

<details>

<summary>30/05 - Selecionar campos do Formulário e Modelo de Documento</summary>

1\. **Workflow > Desenho do Fluxo > Formulário**

A tela de configuração do **formulário** na tarefa, foi alterada para permitir marcar/desmarcar todos os _checkbox’s_ de uma vez.

O comportamento da tela permitia marcar apenas um campo por vez, com esta alteração, em uma tarefa que o usuário precise preencher todos os campos do formulário, será possível marcá-los com apenas um clique.

![](<../.gitbook/assets/image (47).png>)

2\. **Workflow > Desenho do Fluxo > Modelo de Documento**

A tela de configuração do **modelo de documento** na tarefa, foi alterada para permitir marcar/desmarcar todos os _checkbox’s_ de uma vez.

O comportamento da tela permitia marcar apenas um campo por vez, com esta alteração, em uma tarefa que o usuário precise preencher todos os campos do modelo de documento, será possível marcá-los com apenas um clique.

![](<../.gitbook/assets/image (48).png>)

</details>

<details>

<summary>27/05 - Melhoria de Usabilidade - Uso do modelo Formulário em PDF</summary>

O [modelo de documento](https://arquivar.gitbook.io/manual-arqged-or-colaboradores-e-franqueados/workflow/atividades/aba-minhas-atividades#id-7.-modelo-de-documento) foi alterado para dar destaque os campos de preenchimento obrigatórios e não obrigatórios.

</details>

<details>

<summary>23/05 - Inclusão do Menu > API > Gerenciador de Chave de API</summary>

Foi criado em [**Administração um novo Menu chamado API**](https://arquivar.gitbook.io/manual-arqged-or-colaboradores-e-franqueados/administracao/api). Seu objetivo é disponibilizar ao cliente a(s) chave(s) de acesso que será(ão) utilizada(s) para gerenciamento e controle das requisições via API.

</details>

<details>

<summary>23/05 - Contrato - Inclusão de Serviço API</summary>

Foi criado um novo tipo de serviço chamado **ArqAPI.**

Este serviço terá a classificação Software e servirá para [**cobrança das requisições excedentes na utilização da API**](https://arquivar.gitbook.io/manual-arqged-or-colaboradores-e-franqueados/cliente/contratos/aba-servico/exemplos-de-calculo#arqapi) do ArqGED.

![](<../.gitbook/assets/image (42).png>)

</details>

**04/2024**

<details>

<summary>29/04 - Etiqueta e Rótulos - Guarda Interna e Terceirizada</summary>

<mark style="color:green;">**Etiquetas Zebra - Rolo**</mark>

As etiquetas foram alteradas para exibir um QrCode como indicação para encontrar o endereço de uma caixa.

Na imagem abaixo temos uma comparação das etiquetas geradas antes e depois da alteração.

![](<../.gitbook/assets/image (37).png>)

**Demais alterações:**

* Foram removidos os zeros a esquerda do código da caixa;
* Foi mantido o código de barras da caixa, com seu código logo abaixo;
* O código de barras do endereço foi removido mantendo apenas a indicação do endereço;
* A logo do cliente foi reposicionada na horizontal e alinhada com o código do cliente;
* Foi adicionado o QrCode como indicação do endereço de alocação da caixa.
* Quando o endereço da caixa for maior que 3 níveis, haverá uma quebra de linha para atender o espaço da etiqueta.

**Exemplos de Etiquetas Zebra – Rolo para caixa de Cliente (Guarda Interna) com variados tipos de logo:**

![](<../.gitbook/assets/image (38).png>)

**Exemplos de Etiquetas Zebra – Rolo para caixa da Unidade (Guarda Terceirizada):**

A imagem abaixo ilustra uma etiqueta de uma Caixa com as SubCaixas. Somente a subcaixas possuem a indicação “SUBCAIXA”, Caixas Pai ou Caixas que não possuem SubCaixas não possuem a indicação “CAIXA”.

![](<../.gitbook/assets/image (40).png>)

As Etiquetas Zebra – Rolo podem ser retiradas em:

Caixa ou Pasta > Pesquisar > Caixa > Gerar Etiquetas

Caixa ou Pasta > Criar > Caixa do Cliente > Caixa > Gerar Etiquetas. 

Caixa ou Pasta > Criar > Caixa da Unidade > Caixa > Gerar Etiquetas. 

Caixa ou Pasta > Alocar e Desalocar > Caixa do Cliente > Alocar > Gerar Etiqueta

Caixa ou Pasta > Alocar e Desalocar > Caixa da Unidade > Alocar > Gerar Etiqueta

<mark style="color:green;">**Etiquetas – Pimaco 62582**</mark>

As Etiquetas Pimaco foram alteradas para exibir a indicação de código QrCode.

Na imagem abaixo temos uma comparação das etiquetas geradas antes e depois da alteração.

<img src="../.gitbook/assets/image (41).png" alt="" data-size="original">

Demais alterações:

* Foram removidos os zeros a esquerda do código da caixa;
* Foi mantido o código de barras da caixa, com seu código logo abaixo;
* O código de barras do endereço foi removido mantendo apenas a indicação do endereço;
* Foi adicionado o QrCode como indicação do endereço de alocação da caixa.
* Quando o endereço da caixa for maior que 3 níveis, haverá uma quebra de linha para atender o espaço da etiqueta.

<mark style="color:green;">**Rótulos**</mark>

Os rótulos foram alterados para exibir o QrCode como indicação para encontrar o endereço da caixa e removido o código da caixa que era exibido duas vezes.

![](<../.gitbook/assets/image (36).png>)

Os rótulos podem ser retirados em:

Caixa ou Pasta > Pesquisar > Caixa > Gerar Etiquetas

Caixa ou Pasta > Criar > Caixa do Cliente > Caixa > Gerar Etiquetas. 

Caixa ou Pasta > Criar > Caixa da Unidade > Caixa > Gerar Etiquetas. 

Caixa ou Pasta > Alocar e Desalocar > Caixa do Cliente > Alocar > Gerar Etiqueta

Caixa ou Pasta > Alocar e Desalocar > Caixa da Unidade > Alocar > Gerar Etiqueta

</details>

**03/2024**

<details>

<summary>25/03 - Mudança na Cobrança ArqSign no ArqGED e ArqScan</summary>

Foram realizadas melhorias em:

<mark style="color:blue;">**• Faturamento de serviço de ArqSign no ArqGED**</mark>

A apuração da quantidade a faturar para o serviço ArqSIGN no ArqGED foi alterada para considerar apenas arquivos assinados por usuários do cliente, ou seja, assinaturas de usuários da unidade ou da master em qualquer arquivo de documento da árvore documental do cliente não serão contabilizados para o relatório de faturamento.

<mark style="color:blue;">**• Faturamento de Serviço de ArqScan.**</mark>

A apuração da quantidade a faturar para o serviço ArqSCAN foi alterada para considerar apenas arquivos digitalizados por usuários do cliente, ou seja, usuários da unidade ou da master que realizarem digitalização de qualquer arquivo de documento da árvore documental do cliente não será contabilizado para o relatório de faturamento.

</details>

<details>

<summary>18/03 - Contrato - Serviço ArqNFe</summary>

<mark style="color:blue;">**• Cliente > Contrato > Serviço**</mark>

A tela [para adicionar, editar ou visualizar um serviço no contrato,](https://arquivar.gitbook.io/manual-arqged-or-colaboradores-e-franqueados/cliente/contratos/aba-servico#adicionando-um-servico) foi alterada para inclusão de campos exclusivos do ArqNFe.

Quando este serviço for adicionado, serão exibidos os campos “Pacote de referência” e “Valor de referência”.

Estes campos foram criados pra guardar a quantidade e valor para utilização excedente do serviço.

O uso do serviço permanece o mesmo, não houveram alterações na utilização ou forma de cobrança, os campos foram adicionados apenas para referência.

</details>

<details>

<summary>18/03 - Melhoria de Usabilidade: Tela de Reajuste de Contrato</summary>

<mark style="color:blue;">**• Layout da tela Reajustar Contratos.**</mark>

A tela Reajustar os Contratos, foi alterada para destacar as colunas "Novo R$ Periódico" e "Novo R$ Unitário".

A cor de destaque para os valores das colunas irá obedecer a cor do tema escolhido pelo usuário, em negrito.

A alteração visa facilitar visualmente os novos valores dos contratos a serem reajustados quando houver ou não reajuste de valor.

![](<../.gitbook/assets/image (35).png>)

</details>

<details>

<summary>14/03 - Melhorias no Relatório de Faturamento</summary>

<mark style="color:blue;">**• Usabilidade**</mark>

A aplicação foi alterada para diminuir o consumo de processamento na geração dos [**relatórios de faturamento para Unidade e Unidade + Cliente**](https://arquivar.gitbook.io/manual-arqged-or-colaboradores-e-franqueados/faturamento/relatorio)<mark style="color:blue;">**.**</mark>

<mark style="color:blue;">**• Layout do relatório de faturamento.**</mark>

Abaixo os ajustes realizados no layout do relatório de faturamento:

**Coluna Serviços:** A coluna foi alterada para exibir o nome dos serviços com uma quebra de linha e assim ganhar mais espaço para as colunas de preços e quantidades.

**Coluna Qtde dos "Pacote Inicial", "Pacote Periódico" e "Pacote Unitário":** A coluna foi alterada para deixar somente duas casas decimais, com diminuição da coluna para compreender 5 algarismos.

**Colunas Preços:** Houve um aumento destas colunas de forma que o R$ e preço não sejam exibidos com quebra de linha, quando o valor for muito grande.

**Informação de acumulado:** Para os relatórios com informação de acumulado (Saldo utilizado do Pacote Inicial), a informação da quantidade foi incluída abaixo do serviço.

![](<../.gitbook/assets/image (33).png>)

</details>

**02/2024**

<details>

<summary>07/02 - ArqFlow Resiliência para as Notificações</summary>

O envio das notificações do workflow foi alterado para garantir a entrega e eficiência no menor tempo possível.

Houve a **contratação** do serviço de e-mail **SendGrid** que possui foco na entrega das mensagens, além de facilitar a gestão das notificações através de relatórios de envios e falhas. Além deste novo serviço, **continuamos com o SMTP.com e Microsoft 365**, já utilizados anteriormente.

Com **três** possibilidades de **redundância**, criamos um processo para **aumentar a resiliência** das notificações. Caso aconteça alguma eventual falha no serviço principal, a aplicação irá, automaticamente, redirecionar o envio das notificações para algum dos outros serviços disponíveis.

<mark style="color:green;">**Serviço Principal:**</mark> SendGrid

<mark style="color:green;">**Serviços Secundários:**</mark> SMTP.com e Microsoft 365

</details>

**11/2023**

<details>

<summary>10/11 - ArqFlow Ativar fluxo via ArqSCAN</summary>

A ativação de fluxo via ArqSCAN foi alterada para permitir a copia dos dados do registro para os campos do formulário quando estes possuírem os mesmos campos configurados.

Quando é realizado o upload de arquivos no ArqSCAN, é criado um documento com os campos indexadores preenchidos pelo usuário, caso haja ativação de fluxo durante este processo e, o formulário do workflow tenha ao menos um campo igual ao do registro, o seu valor será inserido automaticamente no campo do formulário.

<img src="../.gitbook/assets/Ativação ArqScan.png" alt="" data-size="original">

</details>

<details>

<summary>10/11 - ArqFlow Quem Ativou e Chefe imediato (Quem Ativou)</summary>

A configuração de tarefas para desenhos de fluxos automáticos, baseados em ocorrência “Quando um registro é inserido”, foi alterado para permitir a inclusão dos tipos de responsáveis “Quem Ativou” e “Chefe imediato(Quem Ativou)”.

Anteriormente, estes tipos de responsáveis não eram exibidos para esta configuração de desenho. Os detalhes dessas funcionalidades estão na página [Workflow > Desenho do Fluxo > Configurações da Tarefa.](../workflow/desenho-do-fluxo/aba-fluxograma.md#configuracoes-da-tarefa)

</details>

<details>

<summary>10/11 - ArqIndex Excluir arquivos da pasta processos</summary>

A tela Fluxo de Trabalho foi alterada para inclusão do parâmetro "Deletar os "Arquivos em Processo" após a etapa de conversão".

Atualmente, todos os “Arquivos de Entrada” e “Arquivos em Exportação” são deletados automaticamente pelo robô após a execução de seus respectivos processos (Leitura de XML e Exportação). Para executar o mesmo com os “Arquivos em Processo” é necessário marcar a flag “Deletar os “Arquivos em Processo” após a etapa de conversão”.

O Robô ArqIndex também foi alterado para identificar se irá ou não excluir os arquivos de cada documento, após sua conversão. Os fluxos que apresentarem o parâmetro desmarcado não terão os arquivos de seus documentos excluídos da pasta configurada para o “Arquivos em Processo” no robô.

É necessário solicitar o instalador do ArqIndex junto à Arquivar Master.

</details>

<details>

<summary>10/11 - ArqFlow Excluir fluxos ativos</summary>

A pesquisa por fluxo do workflow foi alterada para adicionar a funcionalidade de exclusão de fluxos ativos. Foi incluído um ícone em cada fluxo no retorno da pesquisa por fluxo.

Os detalhes dessas funcionalidades estão na página [Workflow > Atividades > Aba Pesquisa por Fluxo.](../workflow/atividades/aba-pesquisa-por-fluxo.md)

</details>

**09/2023**

<details>

<summary>14/09 - ArqFlow Bloquear ativação manual sem um documento associado</summary>

A tela [Dados Gerais](../workflow/desenho-do-fluxo/aba-dados-gerais.md) no menu Desenho de um Fluxo foi alterada para incluir o parâmetro “Bloquear a ativação manual deste fluxo sem um documento associado.”

<img src="../.gitbook/assets/dadosgerais_alt01.png" alt="" data-size="original">

Este parâmetro será exibido para seleção somente em desenhos com tipo de ativação manual.

Desenhos de fluxo com este parâmetro selecionado não poderão ser ativados manualmente sem que haja um documento selecionado, ou seja, para estes desenhos um fluxo poderá ser ativado somente via pesquisa simples, avançada, explorar ou aba Workflow na tela de Documentos.

Para ver detalhes dessa funcionalidade acesse [Workflow > Desenho do Fluxo > Aba Dados Gerais.](../workflow/desenho-do-fluxo/aba-dados-gerais.md)

</details>

<details>

<summary>13/09 - ArqFlow Substituição de pessoas</summary>

Na tela de substituição de pessoas, quando o usuário escolher a opção "Substituição Definitiva - Transferir todas as atividades em execução", a aplicação irá verificar todos os fluxos em execução do cliente e enviar todas as tarefas do usuário substituído para o usuário substituto.

Anteriormente, a aplicação substituía o usuário somente nas tarefas em execução do usuário substituído. Com esta alteração, a aplicação irá verificar todos os fluxos que estejam em execução e que já foram executadas por este usuário substituído e, incluir o usuário substituto em todas as tarefas em questão.

Desta forma, quando voltar uma tarefa, esta não irá retornar para o usuário responsável que executou, mas sim para o usuário substituído.

Para ver detalhes dessa funcionalidade acesse [Workflow > Substituição de Pessoas.](../workflow/substituicao-de-pessoas.md#substituicao-definitiva)

</details>

<details>

<summary>13/09 - ArqFlow Grupo de Usuários</summary>

A tela de Grupo de Usuários foi alterada para possibilitar inativar/ativar usuários em um grupo.

Foi incluído um ícone para a funcionalidade e, não será mais necessário excluir um usuário do grupo para que ele não receba tarefas para execução.

Quando for selecionado um usuário do grupo, o ícone será habilitado para que este seja inativado ou ativado, conforme a necessidade.

Usuários inativados em um grupo não irão receber novas tarefas que estejam configuradas para o Grupo em questão.

Para ver detalhes dessa funcionalidade acesse [Workflow > Grupo de Usuários.](../workflow/grupo-de-usuarios.md#inativar-usuarios)

</details>

**08/2023**

<details>

<summary>30/08 - Árvore Organizacional</summary>

A configuração de TTD para um nível de árvore foi alterado para permitir a inclusão de campos do tipo Data de uma lista.

Anteriormente, a configuração de TTD na árvore somente permitia a inclusão de campos customizados do tipo Data.

**Para que seja configurado um campo de lista como configuração de TTD em um nível de árvore será necessário que a lista esteja relacionada nesta árvore.**

</details>

<details>

<summary>30/08 - Pesquisa Avançada e Simples</summary>

As pesquisas avançada e simples foram alteradas para permitir a visualização do Vencimento TTD configurados a partir de um campo de lista na arvore organizacional.

Anteriormente, somente campos customizados possuíam vencimento TTD no documento.

</details>

<details>

<summary>30/08 - ArqFlow TTD antes de vencer em dias</summary>

O desenho de fluxo foi alterado para incluir a opção TTD antes de vencer em dias: para o Tipo de Ativação: Automática e Parâmetro de Ativação: Baseado na TTD.

Anteriormente, a aplicação permitia a possibilidade de ativar fluxos quando um documento ou mais estivessem vencidos, através do parâmetro TTD vencida.

Com esta nova alteração, poderão ser ativados fluxos automáticos para documentos, antes que cheguem o seu vencimento, conforme a quantidade de dias configurada.

**Exemplos:**

* Em um fluxo configurado para ativar diariamente com TTD antes de vencer em dias: 10, a aplicação irá ativar fluxos todos os dias com os documentos que irão vencer em 10 dias, conforme a data de ativação de cada fluxo.
* Em um fluxo configurado para ativar diariamente com TTD antes de vencer em dias: 120, a aplicação irá ativar fluxos todos os dias com os documentos que irão vencer em 120 dias, conforme a data de ativação de cada fluxo.

As configurações de ativação automática de fluxos continuam as mesmas (Diário, Semanal, Mensal), somente foi adicionado esta opção para ativar fluxos com documentos antes de seu vencimento.

Para ver detalhes dessa funcionalidade acesse [Workflow > Desenho do Fluxo> Aba Dados Gerais > Ativação baseada em ocorrências](../workflow/desenho-do-fluxo/aba-dados-gerais.md#ativacao-baseada-em-ocorrencias).

</details>

<details>

<summary>30/08 - ArqFlow Copiar dados de um documento para o Formulário</summary>

A aplicação foi alterada para copiar os dados dos campos de um documento para o formulário, quando estes possuírem os mesmos campos em comum.

**Sempre que houver a ativação de um fluxo relacionado a um documento, a aplicação irá identificar se os campos preenchidos deste documento são os mesmos campos do formulário relacionado ao desenho do fluxo.**

**Caso sejam os mesmos campos, a aplicação irá copiar as informações destes campos e preencher o formulário automaticamente. Quando o usuário abrir o formulário na tarefa, este já estará com seus campos preenchidos.**

**Observação:** O documento e o formulário não precisam ter todos os campos em comum. Caso, o formulário possua ao menos um campo em comum com o documento, seu dado já será copiado para o formulário.

</details>

<details>

<summary>08/08 - API Integração Incluir e alterar dados de um formulário</summary>

Foi adicionado o serviço “api/Workflow/EtapaExecucao/{IdWorkflowEtapaExecucao}/Cliente/{idCliente}/atualizar-dados-formulario” na API Integração Workflow, que permite incluir ou alterar os dados de um formulário a partir da execução de fluxo.

<img src="../.gitbook/assets/api integracao.png" alt="" data-size="original">

**Request:** [https://integracao.arquivar.com/api/Workflow/EtapaExecucao/{IdWorkflowEtapaExecucao}/Cliente/{idCliente}/\
atualizar-dados-formulario](https://integracao.arquivar.com/api/Workflow/EtapaExecucao/%7BIdWorkflowEtapaExecucao%7D/Cliente/%7BidCliente%7D/atualizar-dados-formulario)

Para atualizar os dados de um formulário no workflow será necessário informar obrigatoriamente o “idCliente”, o “IdWorkflowEtapaExecucao”, o “idWorkflow” ou “codigoWorkflow”.

Para alterar ou incluir os dados de um formulário, o fluxo em questão deve estar em execução e o IdWorkflowEtapaExecução deve ser a etapa de execução atual do fluxo.

Para incluir ou alterar qualquer informação de campos de lista, será obrigatório informar o campo chave, o Id da Lista, o Id do Campo e o valor a ser inserido.

**Exemplo:**

<img src="../.gitbook/assets/api integracao 2.png" alt="" data-size="original">

Para incluir ou alterar o campo customizado de um formulário, será obrigatório informar apenas o Id do Campo e o valor a ser inserido, o IdLista deve ficar vazio quando for atualização para valor de campo customizado.

**Exemplo:**

<img src="../.gitbook/assets/api integracao 3.png" alt="" data-size="original">

</details>

07/2023

<details>

<summary>28/07 - ArqFlow Consenso Selecionado Externo Vários</summary>

A aplicação foi alterada para considerar o percentual de consenso em conclusão de tarefas cujo responsável seja “Selecionado Externo Vários”.

Para esta funcionalidade, no desenho do fluxo, a tela de configuração para este Tipo de Responsável foi ajustada para incluir um percentual de consenso para o avanço.

Anteriormente, esse Tipo de Responsável somente era avançado com 100% das execuções e, com esta alteração o usuário poderá definir qual o percentual de execução para o avanço.

Os detalhes dessas funcionalidades estão na página [Workflow > Desenho do Fluxo > Configurações da Tarefa](../workflow/desenho-do-fluxo/aba-fluxograma.md#configuracoes-da-tarefa).

![](<../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png>)

</details>

<details>

<summary>24/07 - ArqFlow Visualizar arquivos selecionados a serem assinados em tarefas externas</summary>

A tela de anexos do fluxo e anexos dos documentos foram alteradas para exibir os arquivos marcados para assinatura em etapas que não há obrigatoriedade de selecionar anexos a serem assinados.

Com esta funcionalidade, a coluna “Assinar” será sempre exibida na tela para que um usuário possa visualizar quais arquivos foram selecionados para serem assinados em tarefas externas.

* Em etapas que houver a obrigatoriedade selecionar os anexos para assinatura, os campos desta coluna serão exibidos habilitados para serem marcados.
* Em etapas que não houver a obrigatoriedade selecionar os anexos para assinatura, os campos desta coluna serão exibidos desabilitados e um usuário poderá visualizar quais arquivos foram marcados em etapas anteriores.

Anteriormente, esta coluna era exibida somente em etapa com obrigatoriedade de selecionar anexos para serem assinados em tarefas externas.

Os detalhes dessas funcionalidades estão na página [Workflow > Atividades > Aba Minhas Atividades > Executando um fluxo](../workflow/atividades/aba-minhas-atividades/executando-um-fluxo.md).

![](<../.gitbook/assets/image (9) (1) (1) (1) (1) (1).png>)

</details>
