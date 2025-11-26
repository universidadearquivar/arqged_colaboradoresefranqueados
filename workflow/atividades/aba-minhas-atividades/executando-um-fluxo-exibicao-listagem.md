# ➡️ Executando um fluxo - Exibição Listagem

## Visualização Listagem

No modo de exibição 'Listagem', os fluxos sob responsabilidade do usuário logado são exibidos de forma simplificada, em uma lista que destaca as informações mais importantes.

Esse modo de visualização pode ser definido como padrão no perfil do usuário, garantindo que, ao acessar a aplicação, a tela de Minhas Atividades seja sempre apresentada nessa configuração.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

A tela será exibida conforme a imagem acima, apresentando as seguintes informações:

#### Barra de Filtro

É possível realizar a busca de tarefas utilizando a barra de filtro, que faz a busca de tarefas do usuário utilizando palavras-chave.

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### Botão Ativar Novo Fluxo

Botão para a ativação de novos fluxos.

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### Gráfico

No topo da tela será exibido um gráfico que permite ao usuário visualizar quantos fluxos estão em atraso, com base no total de fluxos sob sua responsabilidade para execução.

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### Detalhamento das Colunas

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Coluna Nº:** Exibe o número/código do fluxo ou número do processo.

**Coluna Processo:** Exibe o nome do fluxo definido no desenho do processo.

**Coluna Tarefa:** Exibe o nome definido para a tarefa configurada no desenho do fluxo. Ao posicionar o mouse sobre o nome da tarefa, é exibido um _Tooltip_ indicando a situação do fluxo, o status, a classificação (Individual ou Grupo) e as obrigatoriedades com os respectivos botões de avanço. Cada tarefa também possui um ícone que indica o andamento da atividade do usuário: verde para "Em dia", vermelho para "Em atraso" e azul para "atividades delegadas", "aguardando ciência" de outro usuário.

**Coluna Início Tarefa:** Exibe a data/hora de chegada da tarefa para execução do responsável.

**Coluna Concluir Até:** Exibe a previsão de término da atividade, conforme o prazo definido na configuração da tarefa. As etapas de acompanhamento do processo de assinatura via plataforma ArqSIGN não possuem prazo de conclusão e, por esse motivo, são sempre exibidas no topo da lista.

**Coluna Detalhes:** Esta coluna apresenta apenas um ícone. Ao clicar nele, o usuário visualiza uma tela com as informações do fluxo, incluindo os 'Dados Gerais do Processo', a 'Ação da Tarefa Anterior', o nome do responsável que executou a tarefa anterior, o último comentário, os campos do formulário configurados para exibição na tarefa e os 'Dados da Tarefa Atual'. Além disso, a tela também exibe a 'Observação do Fluxo', quando adicionada no momento da ativação, e as 'Instruções para a Tarefa', correspondentes às informações inseridas no campo 'Descrição da Etapa' durante a configuração da tarefa no desenho do fluxo.

**Coluna Ações:** Nesta coluna são exibidos dois botões: o **'Abrir'** e o **'v'**. Ao clicar em **'Abrir'**, uma nova aba é aberta para que o usuário execute as ações da tarefa, como cadastrar ou associar documentos, incluir anexos ao fluxo, preencher formulários, adicionar comentários, entre outras atividades. Ao clicar no botão **'v'**, são exibidos os botões de avanço da tarefa, além das ações 'Abrir Tarefa', 'Delegar Tarefa', 'Cancelar Fluxo', 'Voltar para Tarefa Anterior' e 'Visualizar Fluxograma'.

## Ativar Novo Fluxo

1\. Para ativar um novo fluxo, no menu [Workflow > Atividades > Aba Minhas Atividades](./) clique no botão “Ativar Novo Fluxo”.&#x20;

2\. Informe o nome da empresa no campo “Cliente”.

3\. No campo “Selecione um Processo”, selecione o fluxo que deseja ativar.&#x20;

4\. Se houverem observações, informe-as no campo “Observação”. Caso contrário, deixe o campo em branco. As observações inseridas aqui serão exibidas na tela de execução das tarefas.&#x20;

5\. Selecione se o fluxo terá início imediato (ativar o fluxo no ato) ou se terá o início agendado (com data estabelecida futura).&#x20;

<figure><img src="../../../.gitbook/assets/minhas_ativ02.png" alt=""><figcaption></figcaption></figure>

6. Clique em “Ativar”. Caso seja um fluxo com início agendado, informe a data e hora para ativação e clique em “Agendar”.

<figure><img src="../../../.gitbook/assets/minhas_ativ03.png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
<mark style="color:red;">**Desenhos de fluxo que possuírem o parâmetro "Bloquear a ativação manual deste fluxo sem um documento associado" selecionado (aba Desenho do Fluxo > Aba Dados Gerais), não poderão ser ativados manualmente pelo botão Ativar Novo Fluxo, da aba Minhas Atividades, porque não poderão ser ativados sem que haja um documento selecionado para associação ao fluxo.**</mark>
{% endhint %}

***

### Executando o Fluxo

