# 🟩 Substituição de Pessoas

{% embed url="https://app.supademo.com/demo/cmc281gz1kb4hsn1r4v49cpt7" %}

A funcionalidade de Substituição de Pessoas é utilizada para substituir uma pessoa que estava cadastrada como responsável por uma tarefa em determinado fluxo por outra pessoa, em caso de desligamento, afastamento, transferência de setor etc.

***

## Substituição de Pessoas – Tela Principal

**1. Campo Empresa:** Neste campo é exibida a empresa ou empresas às quais o usuário logado pertence ou tem acesso.&#x20;

**2. Ícone Adicionar:** Utilizado para a criação de uma nova substituição.&#x20;

**3. Ícone Editar:** Utilizado para realizar a edição das informações da substituição selecionada. Só é possível editar substituições provisórias e que ainda não tenham sido realizadas, ou seja, que estão programadas para datas futuras. Substituições passadas e definitivas não podem ser alteradas. &#x20;

**4. Ícone Visualizar:** Utilizado para visualizar detalhes da substituição selecionada. &#x20;

**5. Ícone Excluir:**  Utilizado para excluir a substituição selecionada. Só é possível excluir substituições provisórias e que ainda não tenham sido realizadas, ou seja, que estão programadas para datas futuras. Não é permitido excluir substituições passadas ou definitivas.&#x20;

<figure><img src="../.gitbook/assets/sub5.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Coluna Substituído:** Mostra o nome do usuário que está sendo substituído no fluxo.&#x20;

**Coluna Substituto:** Mostra o nome do usuário substituto, que irá assumir as tarefas do substituído no fluxo. &#x20;

**Coluna Tipo de Substituição:** Mostra se a substituição feita é definitiva ou provisória.&#x20;

**Coluna Data da Substituição/Execução:** Mostra o período em que a substituição provisória está vigente (data inicial e data final) ou, no caso de substituição definitiva, o dia e horário em que foi executada.  &#x20;

<figure><img src="../.gitbook/assets/sub4.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

***

## &#x20;Substituição Provisória

Trata-se de uma alteração realizada por um período determinado de tempo, como nos casos de férias, em que há datas definidas para início e término da substituição. Ao final desse período, os novos fluxos voltam a ser direcionados ao responsável original.

{% hint style="info" %}
<mark style="color:blue;">**Importante:**</mark>

<mark style="color:blue;">•</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Limite de substituição:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Um usuário pode ser definido como substituto em vários fluxos, não existe uma limitação quanto a quantidade de substituições que um único usuário pode fazer.</mark>

<mark style="color:blue;">•</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Associação com Chefe Imediato:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Ao definir um substituto no fluxo de um usuário que seja também chefe imediato, o usuário substituto</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**NÃO**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">se torna chefe imediato. Para isso, é necessário alterar a informação nas Aba de Permissões II de</mark> [<mark style="color:blue;">Chefe Imediato.</mark>](https://manual.arquivar.com/guia-do-cliente/arqged/administracao/usuarios#aba-permissoes-ii)

<p align="center"><img src="https://manual.arquivar.com/guia-do-cliente/~gitbook/image?url=https%3A%2F%2F1023047207-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FtM1xGMYoU6wC7tnUUXEo%252Fuploads%252FU6NOcVyDVOzKoNwLTlZf%252Fimage.png%3Falt%3Dmedia%26token%3Dcc4d1568-28cd-4786-b944-f4a6815eb1d9&#x26;width=300&#x26;dpr=3&#x26;quality=100&#x26;sign=22ecf32d&#x26;sv=2" alt=""></p>
{% endhint %}

Para realizar uma substituição provisória, siga:

1. Clique no ícone “Adicionar”.

<figure><img src="../.gitbook/assets/sub1.png" alt=""><figcaption></figcaption></figure>

2\. Selecione o usuário que será substituído e o usuário substituto nos campos correspondentes.&#x20;

3\. Selecione a opção Substituição Provisória. A substituição provisória ocorrerá só no período indicado no campo “Período da Substituição”.

4\. Selecione as opções desejadas em relação à substituição:&#x20;

* Substituir o usuário em fluxos parametrizados: A substituição será feita em todos os fluxos em que o nome do substituído estiver indicado no desenho do fluxo como responsável por alguma tarefa, mesmo em fluxos que ainda não estão em execução.  &#x20;
* Substituir o usuário em grupos de usuários: A substituição será feita em todos os grupos de usuários em que o substituído estiver incluído, ou seja, o substituto será incluído nesses grupos e executará as tarefas que haviam sido delegadas ao substituído. &#x20;
* Permitir ao substituto executar as tarefas em execução do substituído: O substituto deverá executar tarefas do substituído em fluxos que já estão em execução (em andamento).

5\. Informe o período da substituição e clique em “Ativar”.&#x20;

{% hint style="info" %}
<mark style="color:blue;">É possível alterar ou excluir o período de substituição até um dia antes da data inicial definida. Suponhamos que a substituição tem o período de 20/04 a 30/04. Até 19/04 é possível realizar a alteração ou exclusão da data. Após iniciado o período da substituição, não são permitidas alterações nas datas.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/sub2.png" alt=""><figcaption></figcaption></figure>

***

## Substituição Definitiva

Trata-se de uma alteração sem retorno ao responsável anterior, ou seja definitiva, aplicada em casos como desligamento de colaborador ou promoção para outra função/setor. Nessas situações, os fluxos passam a ser direcionados ao novo responsável de forma permanente ou até que ocorra uma nova definição.

{% hint style="info" %}
<mark style="color:blue;">**Importante:**</mark>

<mark style="color:blue;">•</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Limite de substituição:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Um usuário pode ser definido como substituto em vários fluxos, não existe uma limitação quanto a quantidade de substituições que um único usuário pode fazer.</mark>

<mark style="color:blue;">•</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**Associação com Chefe Imediato:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Ao definir um substituto no fluxo de um usuário que seja também chefe imediato, o usuário substituto</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**NÃO**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">se torna chefe imediato. Para isso, é necessário alterar a informação nas Aba de Permissões II de</mark> [<mark style="color:blue;">Chefe Imediato.</mark>](https://manual.arquivar.com/guia-do-cliente/arqged/administracao/usuarios#aba-permissoes-ii)

<p align="center"><img src="https://manual.arquivar.com/guia-do-cliente/~gitbook/image?url=https%3A%2F%2F1023047207-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FtM1xGMYoU6wC7tnUUXEo%252Fuploads%252FU6NOcVyDVOzKoNwLTlZf%252Fimage.png%3Falt%3Dmedia%26token%3Dcc4d1568-28cd-4786-b944-f4a6815eb1d9&#x26;width=300&#x26;dpr=3&#x26;quality=100&#x26;sign=22ecf32d&#x26;sv=2" alt=""></p>
{% endhint %}

Para realizar uma substituição definitiva, siga:

1. Clique no ícone “Adicionar”.

<figure><img src="../.gitbook/assets/sub1.png" alt=""><figcaption></figcaption></figure>

2\. Selecione o usuário que será substituído e o usuário substituto nos campos correspondentes.&#x20;

3\. Selecione a opção Substituição Definitiva. No caso da substituição definitiva será feita uma mudança no banco de dados, ou seja, o substituído será excluído de todos os fluxos e tarefas em que estiver indicado como responsável e o nome do substituto será inserido.&#x20;

4\. Selecione as opções desejadas em relação à substituição:&#x20;

* Substituir o usuário em fluxos parametrizados: A substituição será feita em todos os fluxos em que o nome do substituído estiver indicado no desenho do fluxo como responsável por alguma tarefa, mesmo em fluxos que ainda não estão em execução.  &#x20;
* Substituir o usuário em grupos de usuários: A substituição será feita em todos os grupos de usuários em que o substituído estiver incluído, ou seja, o substituto será incluído nesses grupos e executará as tarefas que haviam sido delegadas ao substituído. &#x20;
* Transferir todas as atividades em execução: O sistema irá verificar todos os fluxos em execução do cliente e enviar todas as tarefas do usuário substituído para o usuário substituto. Caso uma tarefa precise retornar para execução, será encaminhada para o usuário substituto.&#x20;

5. A data da execução será preenchida automaticamente no momento em que o usuário clicar em “Executar”.

<figure><img src="../.gitbook/assets/sub3.png" alt=""><figcaption></figcaption></figure>

