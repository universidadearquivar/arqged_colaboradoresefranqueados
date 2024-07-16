# ▫️ Novembro | 2023



<details>

<summary>10/11: ArqFlow - Ativar fluxo via ArqSCAN</summary>

A ativação de fluxo via ArqSCAN foi alterada para permitir a copia dos dados do registro para os campos do formulário quando estes possuírem os mesmos campos configurados.&#x20;

Quando é realizado o upload de arquivos no ArqSCAN, é criado um documento com os campos indexadores preenchidos pelo usuário, caso haja ativação de fluxo durante este processo e, o formulário do workflow tenha ao menos um campo igual ao do registro, o seu valor será inserido automaticamente no campo do formulário.

<img src="../.gitbook/assets/Ativação ArqScan.png" alt="" data-size="original">

</details>

<details>

<summary>10/11: ArqFlow - Quem Ativou e Chefe imediato (Quem Ativou)</summary>

A configuração de tarefas para desenhos de fluxos automáticos, baseados em ocorrência “Quando um registro é inserido”, foi alterado para permitir a inclusão dos tipos de responsáveis “Quem Ativou” e “Chefe imediato(Quem Ativou)”.&#x20;

Anteriormente, estes tipos de responsáveis não eram exibidos para esta configuração de desenho. Os detalhes dessas funcionalidades estão na página [Workflow > Desenho do Fluxo > Configurações da Tarefa.](../workflow/desenho-do-fluxo/aba-fluxograma.md#configuracoes-da-tarefa)

</details>

<details>

<summary>10/11: ArqIndex – Excluir arquivos da pasta processos</summary>

A tela Fluxo de Trabalho foi alterada para inclusão do parâmetro "Deletar os "Arquivos em Processo" após a etapa de conversão".

Atualmente, todos os “Arquivos de Entrada” e “Arquivos em Exportação” são deletados automaticamente pelo robô após a execução de seus respectivos processos (Leitura de XML e Exportação). Para executar o mesmo com os “Arquivos em Processo” é necessário marcar a flag “Deletar os “Arquivos em Processo” após a etapa de conversão”.&#x20;

O Robô ArqIndex também foi alterado para identificar se irá ou não excluir os arquivos de cada documento, após sua conversão. Os fluxos que apresentarem o parâmetro desmarcado não terão os arquivos de seus documentos excluídos da pasta configurada para o “Arquivos em Processo” no robô.&#x20;

É necessário solicitar o instalador do ArqIndex junto à Arquivar Master.

</details>

<details>

<summary>10/11: ArqFlow – Excluir fluxos ativos</summary>

A pesquisa por fluxo do workflow foi alterada para adicionar a funcionalidade de exclusão de fluxos ativos. Foi incluído um ícone em cada fluxo no retorno da pesquisa por fluxo.

Os detalhes dessas funcionalidades estão na página [Workflow > Atividades > Aba Pesquisa por Fluxo.](../workflow/atividades/aba-pesquisa-por-fluxo.md)

</details>
