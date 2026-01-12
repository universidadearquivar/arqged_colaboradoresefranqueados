# 🟩 Horários de Trabalho

{% embed url="https://app.supademo.com/demo/cmacv3p167ro913m0k48e2mox" %}

O menu Horários de Trabalho objetiva sinalizar ao sistema informações importantes que devem ser consideradas sobre o prazo de execução das tarefas. Neste menu deve ser cadastrado o horário de expediente das unidades e setores da empresa.

O cadastro dos horários de trabalho é importante para que o sistema considere o expediente da empresa ou de um funcionário ao fazer a contagem do prazo para execução das tarefas. Empresas com mais de uma unidade, por exemplo, podem ter expedientes diferentes, ou mesmo setores de uma mesma unidade podem funcionar em horários distintos.

{% hint style="info" %}
<mark style="color:blue;">**EXEMPLO:**</mark> <mark style="color:blue;">Se um funcionário da empresa trabalha das 8h às 17h e no fim do seu expediente recebe uma tarefa que precisa ser executada em quatro horas, o sistema irá desconsiderar as horas em que ele não está trabalhando e só começará a contar o prazo a partir de 8h do dia seguinte.</mark>
{% endhint %}

***

## Horários de Trabalho – Tela principal

**1. Campo Empresa:** Neste campo é exibida a empresa ou empresas às quais o usuário logado pertence ou tem acesso.

**2. Ícone Adicionar:** Utilizado para o cadastro de um novo horário de trabalho. Uma mesma empresa ou unidade pode contar com horários de trabalho distintos.

**3. Ícone Editar:** Utilizado para realizar a edição do horário de trabalho selecionado.

**4. Ícone Visualizar:** Utilizado para visualizar detalhes do horário de trabalho selecionado.

**5. Ícone Excluir:** Utilizado para excluir o horário de trabalho selecionado.

**6. Ícone Selecionar como padrão para usuários externos:** Utilizado para selecionar um dos horários de trabalho como padrão ao considerar o prazo de execução das tarefas por um usuário externo. Esse parâmetro será utilizado durante a Configuração das Tarefas no Desenho do Fluxo.

**7. Coluna Nome do Horário de Trabalho:** Nesta coluna são exibidos todos os horários de trabalho da empresa cadastrados.

**8. Coluna Para Usuários Externos:** Nesta coluna é mostrado qual dos horários de trabalho da empresa está sendo utilizado como padrão no direcionamento de tarefas para usuários externos.

<figure><img src="../.gitbook/assets/horario01.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Usuários externos são aqueles que executam tarefas no processo fora do ArqGED (deslogados), como fornecedores, clientes etc.**</mark>
{% endhint %}

***

## Cadastro de Horários de Trabalho

1. Clique no ícone “Adicionar”.

<figure><img src="../.gitbook/assets/horario02.png" alt=""><figcaption></figcaption></figure>

2. Insira um nome para o horário de trabalho.

<figure><img src="../.gitbook/assets/horario03.png" alt=""><figcaption></figcaption></figure>

3. Selecione o primeiro dia da semana que irá compor aquele expediente e insira os horários de início e fim da jornada e início e fim do intervalo.

<figure><img src="../.gitbook/assets/horario04.png" alt=""><figcaption></figcaption></figure>

4. Para replicar os horários nos demais dias da semana, clique no ícone “Copiar valores para os dias vazios”.

<figure><img src="../.gitbook/assets/horario05.png" alt=""><figcaption></figcaption></figure>

5. Todos os dias da semana serão preenchidos. Desmarque aqueles que não devem ser contabilizados.

<figure><img src="../.gitbook/assets/horario06.gif" alt=""><figcaption></figcaption></figure>

6\. Se não houver intervalo em determinado dia, insira apenas o início e fim da jornada.

7\. Concluído o cadastro, clique em “Salvar”.

<figure><img src="../.gitbook/assets/horario07.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**A atribuição do horário de trabalho de cada usuário deve ser feita no menu Administração > Usuários > Aba Permissões II.**</mark>
{% endhint %}
