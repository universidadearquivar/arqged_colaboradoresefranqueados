# 🟩 Campo Customizado

{% @supademo/embed demoId="cmamwj92212tv2gbpvjdjlfuc" url="https://app.supademo.com/demo/cmamwj92212tv2gbpvjdjlfuc" %}

Os campos customizados são indexadores criados para identificar o conteúdo do documento que permite localizar um arquivo com maior rapidez e precisão a partir do cruzamento de informações.

Ao se decidir criar um tipo documental é preciso ​definir quais campos vão compor aquele documento e servirão como indexadores. Esses campos devem ser criados neste menu. Um mesmo campo customizado pode ser usado em mais de um tipo documental. Para exibir os campos customizados criados para um cliente, selecione-o no campo “Cliente”.

<figure><img src="../.gitbook/assets/arvore8.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">**EXEMPLO:**</mark> <mark style="color:blue;">Ao criar o tipo documental Nota Fiscal, os campos “Número” e “Data” serão alguns dos</mark> <mark style="color:blue;">**campos customizados**</mark> <mark style="color:blue;">que deverão compor o documento e serão utilizados como indexadores para a localização das notas fiscais no sistema.</mark>
{% endhint %}

***

## Campo customizado - Tela principal

**Ícone Adicionar:** Utilizado para cadastrar um novo campo customizado.

**Ícone Editar:** Utilizado para editar as informações do campo customizado selecionado.

**Ícone Visualizar:** Utilizado para apresentar as informações do campo customizado selecionado.

**Ícone Excluir:** Utilizado para excluir o campo customizado selecionado.

<figure><img src="../.gitbook/assets/arvoredoc07.png" alt=""><figcaption></figcaption></figure>

**Coluna Nome:** Apresenta o nome do campo.

**Coluna Definição do Campo:** Apresenta o formato do campo.

**Coluna Expressão:** Apresenta a expressão regular utilizada para validar o campo, se houver.

**Coluna Máscara:** Apresenta a máscara definida para preenchimento do campo, se houver.

**Coluna Campo Pai:** Apresenta o campo pai do qual aquele campo é derivado, se houver.

<figure><img src="../.gitbook/assets/arvoredoc08.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Cadastro de Campo Customizado

Clique no ícone “Adicionar”.

<figure><img src="../.gitbook/assets/arvoredoc09.png" alt=""><figcaption></figcaption></figure>

Informe o nome do campo. Em “Definição de Campo” selecione se o formato do campo, que pode ser:

* _Checkbox:_ Campo em que o usuário deverá marcar uma caixa de seleção de acordo com a pergunta apresentada.
* _CNPJ:_ Campo em que o usuário deverá informar um número de CNPJ válido.
* _CNPJ/CPF:_ Campo em que o usuário deverá informar um número de CNPJ ou de CPF válido.
* _CPF:_ Campo em que o usuário deverá informar um número de CPF válido.
* _Data:_ O usuário deverá informar uma data válida, com dia, mês e ano.
* _Lista:_ Deverá ser criada uma lista de opções para que o usuário selecione a opção que deseja.
  * Aqui, por exemplo, podem ser incluídos em lista novos prestadores aprovados para executar determinado serviço.
* _Monetário:_ Campo em que o usuário deverá informar um valor monetário, com vírgula.
* _Numérico:_ Campo em que o usuário deverá informar um valor numérico.
* _Texto:_ Campo em que o usuário poderá informar qualquer valor, seja de texto ou numérico. Este tipo de campo aceita qualquer caractere como resposta.

<figure><img src="../.gitbook/assets/arvoredoc10.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Expressão:** No campo Expressão pode ser informada uma expressão regular para verificar o preenchimento do campo.

{% hint style="info" %}
<mark style="color:blue;">Uma</mark> <mark style="color:blue;">**expressão regular**</mark> <mark style="color:blue;">é usada para verificar se uma cadeia de caracteres contém o padrão de busca especificado. Por exemplo, se for preciso que o usuário informe um número de celular brasileiro válido, pode-se aplicar uma expressão regular para a pergunta. Ao fazer isso, todos os respondentes terão que inserir os números de celulares correspondentes ao formato do número de celular brasileiro - (xx) xxxxx-xxxx. Se o número de telefone não corresponder a esse padrão, será exibida uma mensagem de erro indicando que ele deve corresponder ao formato apropriado.</mark>
{% endhint %}

**Máscara:** No campo Máscara deverá ser informado o formato da resposta aceita, se houver um formato obrigatório. Neste caso, a letra X deve representar a quantidade de letras requeridas e o número 9 a quantidade de números. Se houver um dígito verificador, utilize o hífen (-).

{% hint style="info" %}
<mark style="color:blue;">**EXEMPLO:**</mark> <mark style="color:blue;">Se for solicitado que a resposta contenha obrigatoriamente quatro letras, um dígito e quatro números, no campo Máscara informe “XXXX-9999”.</mark>
{% endhint %}

**Tamanho mínimo:** No campo tamanho mínimo pode ser informado a quantidade mínima de caracteres do campo.

**Tamanho máximo:** No campo tamanho máximo pode ser informado a quantidade máxima de caracteres do campo.

{% hint style="info" %}
<mark style="color:blue;">**Exemplo:**</mark> <mark style="color:blue;">se a definição de um campo for para o preenchimento de uma data, e o sistema aceitar diferentes formatos como</mark> <mark style="color:blue;">`ddmmaa`</mark><mark style="color:blue;">,</mark> <mark style="color:blue;">`ddmmaaaa`</mark> <mark style="color:blue;">ou</mark> <mark style="color:blue;">`dd/mm/aaaa`</mark><mark style="color:blue;">, é possível definir um comprimento mínimo de 6 caracteres e máximo de 10 caracteres. Isso garante flexibilidade na entrada do dado sem comprometer a validação da informação.</mark>
{% endhint %}

**Operador:** O campo **Operador** é utilizado para estabelecer uma condição de dependência entre o **Campo Pai** e o campo atual. Ele define a lógica de comparação que será aplicada ao valor informado no **Campo Pai** para que o campo atual seja habilitado para preenchimento.

Os operadores disponíveis são:

* `=`   (igual a)
* `>`   (maior que)
* `<`   (menor que)
* `>=`  (maior ou igual a)
* `<=`  (menor ou igual a)
* `<>`  (entre)

Essa configuração é útil em cenários em que o campo que está sendo criado depende de uma condição prévia estabelecida no **Campo Pai**. Somente quando essa condição for atendida — ou seja, quando o valor informado no Campo Pai satisfizer o operador e o valor definidos — o novo campo será liberado para preenchimento.

{% hint style="info" %}
<mark style="color:blue;">**Exemplo:**</mark>\ <mark style="color:blue;">Se o</mark> <mark style="color:blue;">**Campo Pai**</mark> <mark style="color:blue;">for “Idade”, o</mark> <mark style="color:blue;">**Operador**</mark> <mark style="color:blue;">for</mark> <mark style="color:blue;">`>=`</mark> <mark style="color:blue;">e o valor definido for</mark> <mark style="color:blue;">`18`</mark><mark style="color:blue;">, o campo atual só será exibido quando o usuário informar no campo “Idade” um valor maior ou igual a 18.</mark>
{% endhint %}

**Campo Pai:** O Campo Pai é aquele do qual o campo atual depende para ser exibido ou habilitado. Ao selecionar um Campo Pai, você estabelece uma relação de dependência condicional: o campo que está sendo configurado só ficará disponível para preenchimento se o Campo Pai for previamente preenchido e atender à condição definida pelo Operador e o Valor de Referência.

Essa funcionalidade permite criar fluxos de preenchimento mais inteligentes, nos quais certos campos só aparecem ou se tornam obrigatórios conforme o contexto fornecido pelo usuário.

{% hint style="warning" %}
<mark style="color:orange;">**Importante:**</mark>

* <mark style="color:orange;">A seleção de um Campo Pai exige que também sejam definidos um</mark> <mark style="color:orange;">**Operador**</mark> <mark style="color:orange;">e um</mark> <mark style="color:orange;">**Valor de Referência**</mark><mark style="color:orange;">, que juntos determinam a lógica de exibição do campo.</mark>
* <mark style="color:orange;">Se o Campo Pai não for preenchido, ou se o valor informado não atender à condição configurada, o campo dependente permanecerá oculto ou desabilitado.</mark>
* <mark style="color:orange;">**Para que a associação entre campos funcione corretamente, ambos os campos (Campo Pai e campo dependente) devem possuir a mesma definição de tipo.**</mark>\ <mark style="color:orange;">Por exemplo: para que “Data Final > Data Inicial” seja uma condição válida, os dois campos precisam estar definidos como do tipo</mark> <mark style="color:orange;">**Data**</mark><mark style="color:orange;">.</mark>
{% endhint %}

{% hint style="info" %}
<mark style="color:blue;">**Exemplo:**</mark>\ <mark style="color:blue;">Se o Campo Pai for “Tipo de Pessoa” e o valor esperado for “Jurídica”, o campo “CNPJ” (campo atual) só será exibido quando o usuário selecionar “Jurídica” no campo “Tipo de Pessoa”.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/arvoredoc11.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Edição de Campo Customizado

<figure><img src="../.gitbook/assets/image (324).png" alt="" width="361"><figcaption></figcaption></figure>

Ao clicar em **“Editar”**, você poderá **alterar os dados de um registro**.

{% hint style="warning" %}
<mark style="color:orange;">**Importante:**</mark> <mark style="color:orange;">As opções de edição</mark> <mark style="color:orange;">**vão depender da Definição de Campo**</mark> <mark style="color:orange;">escolhida no momento da criação do registro.</mark>
{% endhint %}

* _**Checkbox:**_ Campo em que o usuário deverá marcar uma caixa de seleção de acordo com a pergunta apresentada. É possível alterar a Definição de Campo, Nome do registro, Expressão, Tamanho Mínimo, Tamanho Máximo, Operador e Campo Pai.

<div align="left"><figure><img src="../.gitbook/assets/image (326).png" alt="" width="375"><figcaption></figcaption></figure></div>

* _**CNPJ:**_ Campo em que o usuário deverá informar um número de CNPJ válido. É possível alterar o Nome do registro, Expressão, Tamanho Mínimo, Tamanho Máximo, Operador e Campo Pai.

<div align="left"><figure><img src="../.gitbook/assets/image (327).png" alt="" width="375"><figcaption></figcaption></figure></div>

* _**CNPJ/CPF:**_ Campo em que o usuário deverá informar um número de CNPJ ou de CPF válido. É possível alterar a Definição de Campo, Nome do registro, Expressão, Tamanho Mínimo, Tamanho Máximo, Operador e Campo Pai.

<div align="left"><figure><img src="../.gitbook/assets/image (328).png" alt="" width="375"><figcaption></figcaption></figure></div>

* _**CPF:**_ Campo em que o usuário deverá informar um número de CPF válido. É possível alterar a Definição de Campo, Nome do registro, Expressão, Tamanho Mínimo, Tamanho Máximo, Operador e Campo Pai.

<div align="left"><figure><img src="../.gitbook/assets/image (329).png" alt="" width="375"><figcaption></figcaption></figure></div>

* _**Data:**_ O usuário deverá informar uma data válida, com dia, mês e ano. É possível alterar a Definição de Campo, Nome do registro, Expressão, Tamanho Mínimo, Tamanho Máximo, Operador e Campo Pai.

<div align="left"><figure><img src="../.gitbook/assets/image (330).png" alt="" width="375"><figcaption></figcaption></figure></div>

* _**Lista:**_ Deverá ser criada uma lista de opções para que o usuário selecione a opção que deseja.
  * Aqui, por exemplo, podem ser incluídos em lista novos prestadores aprovados para executar determinado serviço. É possível alterar a Definição de Campo, Nome do registro.
  * **Adicionar lista de valores para o campo:** clique no ícone "+" para adicionar o nome da lista desejada e, caso queira retirar alguma lista, selecione a lista desejada e clique no ícone de lixeira para eliminá-la da lista.

<div align="left"><figure><img src="../.gitbook/assets/image (331).png" alt="" width="375"><figcaption></figcaption></figure></div>

* _**Monetário:**_ Campo em que o usuário deverá informar um valor monetário, com vírgula. É possível alterar a Definição de Campo, Nome do registro, Expressão, Tamanho Mínimo, Tamanho Máximo, Operador e Campo Pai.

<div align="left"><figure><img src="../.gitbook/assets/image (332).png" alt="" width="375"><figcaption></figcaption></figure></div>

* _**Numérico:**_ Campo em que o usuário deverá informar um valor numérico. É possível alterar o Nome do registro, Expressão, Tamanho Mínimo, Tamanho Máximo, Operador e Campo Pai.

<div align="left"><figure><img src="../.gitbook/assets/image (333).png" alt="" width="375"><figcaption></figcaption></figure></div>

* _**Texto:**_ Campo em que o usuário poderá informar qualquer valor, seja de texto ou numérico. Este tipo de campo aceita qualquer caractere como resposta. É possível alterar o Nome do registro, Expressão, Tamanho Mínimo, Tamanho Máximo, Operador e Campo Pai.

<div align="left"><figure><img src="../.gitbook/assets/image (334).png" alt="" width="375"><figcaption></figcaption></figure></div>
