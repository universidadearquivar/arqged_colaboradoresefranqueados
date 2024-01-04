# 🟩 Criar Listas

Neste menu são criadas as listas do cliente selecionado no campo “Cliente”. &#x20;

<figure><img src="../.gitbook/assets/lista01.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Criar Listas - Tela principal&#x20;

**Ícone Adicionar:** Utilizado para cadastrar uma nova lista.

**Ícone Editar:** Utilizado para editar as informações da lista selecionada.

**Ícone Visualizar:** Utilizado para apresentar as informações da lista selecionada.&#x20;

**Ícone Excluir:** Utilizado para excluir a lista selecionada.

<figure><img src="../.gitbook/assets/lista021.png" alt=""><figcaption></figcaption></figure>

**Coluna Cliente:** Exibe o nome do cliente escolhido no campo “Cliente”.

**Coluna Nome da lista:** Exibe o nome da lista.

**Coluna Nome da lista pai:** Caso a lista seja subordinada a outra, neste campo será exibido o nome da lista pai.

**Coluna Status:** Informa se a lista está ativa ou inativa.

<figure><img src="../.gitbook/assets/lista03.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Criando uma lista

Clique no ícone “Adicionar”.

<figure><img src="../.gitbook/assets/lista04.png" alt=""><figcaption></figcaption></figure>

**Nome da Lista:** Informe o um nome para a lista que está sendo criada.

Tipo de lista: Selecione o tipo de lista, que pode ser “Auto Complete” ou “Consolidação”. Quando é necessário que o sistema faça a conferência de algum item da lista, ou seja, se é necessária auditoria, deve ser escolhida a opção “Consolidação”. A lista de Auto Complete não pode ser utilizada para auditoria.&#x20;

{% hint style="info" %}
<mark style="color:blue;">**EXEMPLO:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Em uma lista de funcionários é necessário que o sistema faça constantemente a conferência para verificar se não há documentos obrigatórios faltantes. Neste caso, a lista de funcionários deve ser do tipo “Consolidação”.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/lista05.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Status:** Informe se a lista ficará ativa ou inativa.

<figure><img src="../.gitbook/assets/lista06.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Esta lista é uma lista de um item da lista de:** Este campo só será habilitado se a lista for do tipo “Consolidação”. Neste caso, a lista que está sendo criada poderá ser uma sub lista de outra (lista pai), que deve ser selecionada neste campo.

{% hint style="info" %}
<mark style="color:blue;">**EXEMPLO:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Na lista “Funcionários” existem os campos Matrícula (campo chave), Nome, Função, Admissão e Demissão. Para saber quando um funcionário deverá receber um recibo de férias, foi criada a lista “Férias”, que será filha da lista “Funcionários”, ou seja, utilizará o mesmo campo chave (Matrícula), além de campos específicos da lista como Início das Férias e Fim das Férias. Para saber quando deverá ser enviado um recibo de férias, será criada uma regra de auditoria baseada na lista “Férias”.</mark>
{% endhint %}

**Permitir a inclusão durante a indexação:** Esta opção só ficará disponível se a lista for do tipo “Consolidação”. A lista de Consolidação permite a inclusão de informações durante a indexação, ou seja, se no momento de cadastrar um documento composto por uma lista eu informar um dado de pessoa ou empresa ainda não informado anteriormente, o sistema permitirá que eu insira os dados manualmente naquele momento. A partir daí, nas próximas vezes que utilizar um documento com essa mesma lista, ele extrairá as informações automaticamente. Na lista Auto Complete só é permitido incluir informações antes da indexação, como itens de lista. A inclusão de itens após a indexação deverá ser feita via API ou por meio de importação de dados do Excel add-in. &#x20;

<figure><img src="../.gitbook/assets/lista07.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Ao clicar em “Salvar” será exibida a área “Campos da Lista”, onde deverão ser criados os campos que vão compor a lista que está sendo criada.

<figure><img src="../.gitbook/assets/lista08.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Para cadastrar um campo clique no ícone “Editar” e informe o nome do campo que está sendo criado.

<figure><img src="../.gitbook/assets/lista09.png" alt=""><figcaption></figcaption></figure>
