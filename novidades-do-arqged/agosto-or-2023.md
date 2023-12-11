# ▫ Agosto | 2023

<details>

<summary>30/08: Árvore Organizacional</summary>

A configuração de TTD para um nível de árvore foi alterado para permitir a inclusão de campos do tipo Data de uma lista.

Anteriormente, a configuração de TTD na árvore somente permitia a inclusão de campos customizados do tipo Data.

**Para que seja configurado um campo de lista como configuração de TTD em um nível de árvore será necessário que a lista esteja relacionada nesta árvore.**

</details>

<details>

<summary>30/08: Pesquisa Avançada e Simples</summary>

As pesquisas avançada e simples foram alteradas para permitir a visualização do Vencimento TTD configurados a partir de um campo de lista na arvore organizacional.

Anteriormente, somente campos customizados possuíam vencimento TTD no documento.

</details>

<details>

<summary>30/08: ArqFlow - TTD antes de vencer em dias</summary>

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

<summary>30/08: ArqFlow - Copiar dados de um documento para o Formulário</summary>

A aplicação foi alterada para copiar os dados dos campos de um documento para o formulário, quando estes possuírem os mesmos campos em comum.

**Sempre que houver a ativação de um fluxo relacionado a um documento, a aplicação irá identificar se os campos preenchidos deste documento são os mesmos campos do formulário relacionado ao desenho do fluxo.**

**Caso sejam os mesmos campos, a aplicação irá copiar as informações destes campos e preencher o formulário automaticamente. Quando o usuário abrir o formulário na tarefa, este já estará com seus campos preenchidos.**

**Observação:** O documento e o formulário não precisam ter todos os campos em comum. Caso, o formulário possua ao menos um campo em comum com o documento, seu dado já será copiado para o formulário.

</details>

<details>

<summary>08/08: API Integração Incluir e alterar dados de um formulário</summary>

Foi adicionado o serviço “api/Workflow/EtapaExecucao/{IdWorkflowEtapaExecucao}/Cliente/{idCliente}/atualizar-dados-formulario” na API Integração Workflow, que permite incluir ou alterar os dados de um formulário a partir da execução de fluxo.

<img src="../.gitbook/assets/api integracao.png" alt="" data-size="original">

**Request:** [https://integracao.arquivar.com/api/Workflow/EtapaExecucao/{IdWorkflowEtapaExecucao}/Cliente/{idCliente}/\
atualizar-dados-formulario](https://integracao.arquivar.com/api/Workflow/EtapaExecucao/%7BIdWorkflowEtapaExecucao%7D/Cliente/%7BidCliente%7D/atualizar-dados-formulario)

Para atualizar os dados de um formulário no workflow será necessário informar obrigatoriamente o “idCliente”, o “IdWorkflowEtapaExecucao”, o “idWorkflow” ou “codigoWorkflow”.&#x20;

Para alterar ou incluir os dados de um formulário, o fluxo em questão deve estar em execução e o IdWorkflowEtapaExecução deve ser a etapa de execução atual do fluxo.&#x20;

Para incluir ou alterar qualquer informação de campos de lista, será obrigatório informar o campo chave, o Id da Lista, o Id do Campo e o valor a ser inserido.

**Exemplo:**

<img src="../.gitbook/assets/api integracao 2.png" alt="" data-size="original">

Para incluir ou alterar o campo customizado de um formulário, será obrigatório informar apenas o Id do Campo e o valor a ser inserido, o IdLista deve ficar vazio quando for atualização para valor de campo customizado.

**Exemplo:**&#x20;

<img src="../.gitbook/assets/api integracao 3.png" alt="" data-size="original">

</details>
