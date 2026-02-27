# 🟩 Estrutura Organizacional

{% embed url="https://app.supademo.com/demo/cmal0r36435ym10snj6b74p5h" %}

Estrutura organizacional é a nomeação da dada à estrutura física da empresa do cliente. Neste menu são nomeados os setores, unidades, documentos e outros elementos que compõem a estrutura da empresa.&#x20;

{% hint style="warning" %}
<mark style="color:orange;">**É importante que no momento de criar a estrutura organizacional do cliente o seu projeto de implantação já esteja pronto, para direcionar como essa estrutura deverá ser organizada de acordo com a estrutura física existente na empresa cliente.**</mark>
{% endhint %}

A estrutura organizacional deve ser cadastrada uma única vez, mesmo sendo utilizada por diversas árvores documentais. Para exibir a estrutura de um cliente, selecione-o no campo “Cliente”.&#x20;

<figure><img src="../.gitbook/assets/arvore5.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">**EXEMPLO:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Uma empresa possui três filiais. Sua</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**estrutura do cliente**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">é composta pelos</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**tipos de estrutura:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Filial, Departamento e Documentos. Sua</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**estrutura organizacional**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">é composta pela Filial Belo Horizonte, Filial Salvador e Filial São Paulo, pelos Departamentos RH, Comercial e Financeiro e pelos Documentos Contrato, Ficha de Funcionário e Nota Fiscal.</mark>
{% endhint %}

***

## Estrutura Organizacional - Tela principal

**Coluna Nome do Tipo de Estrutura:** Exibe o Tipo de Estrutura à qual a Estrutura Organizacional selecionada foi associada.&#x20;

**Coluna Nome da Estrutura Organizacional:** Exibe o nome dado à Estrutura Organizacional selecionada.&#x20;

**Coluna Código:** Informa o código utilizado para identificar a Estrutura Organizacional. &#x20;

<figure><img src="../.gitbook/assets/arvore6.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Ícone Adicionar:** Utilizado para cadastrar um novo tipo de Estrutura Organizacional.  &#x20;

**Ícone Editar:** Utilizado para editar as informações do tipo de estrutura selecionado.&#x20;

**Ícone Visualizar:** Utilizado para apresentar as informações do tipo de estrutura. &#x20;

**Ícone Excluir:** Utilizado para excluir o tipo de estrutura selecionado.&#x20;

<figure><img src="../.gitbook/assets/arvore7.png" alt=""><figcaption></figcaption></figure>

***

## Cadastro de Estrutura Organizacional&#x20;

Selecione o cliente para o qual será elaborada a estrutura organizacional e clique no ícone “Adicionar”. &#x20;

<figure><img src="../.gitbook/assets/arvoredoc05.png" alt=""><figcaption></figcaption></figure>

Selecione o Tipo de Estrutura que será utilizado. Os tipos de estrutura apresentados aqui foram criados anteriormente no menu [Tipo de Estrutura](tipo-de-estrutura.md).  &#x20;

Informe o nome da Estrutura Organizacional.

{% hint style="info" %}
<mark style="color:blue;">**EXEMPLO:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Se selecionado o tipo de estrutura “Filial”, informe o nome da cidade da filial: Belo Horizonte, São Paulo etc. Se selecionado o tipo de estrutura “Setor”, informe o nome do setor que está sendo cadastrado: RH, Comercial, Financeiro etc.</mark>
{% endhint %}

Se no momento da criação da [Estrutura do Cliente](estrutura-do-cliente.md) tiver sido definido que será usada codificação para identificar a estrutura, o campo “Código” será mostrado. Informe um código numérico para identificar o item da estrutura organizacional que está sendo cadastrado.

{% hint style="info" %}
<mark style="color:blue;">O</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**código numérico**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">geralmente é utilizado quando a empresa utiliza uma tabela de classificação documental para a organização de seus documentos, como por exemplo a utilizada pelo CONARQ.</mark> [<mark style="color:blue;">**Clique aqui**</mark>](https://www.gov.br/arquivonacional/pt-br/servicos/gestao-de-documentos/orientacao-tecnica-1/codigo-de-classificacao-e-tabela-de-temporalidade-e-destinacao-de-documentos-de-arquivo/copy_of_cod_classif_-e_tab_temp_2019_m_book_digital_25jun2020.pdf) <mark style="color:blue;">e confira.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/arvoredoc06.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Indexação Automatizada:** Quando este parâmetro estiver marcado para uma Estrutura Organizacional, significa que o usuário poderá configurar na Tela da Árvore Organizacional, para esta estrutura, quais extensões de arquivos serão obrigadas para uma indexação via API.

&#x20;Ou seja, em uma Árvore Organizacional, o usuário poderá configurar que na criação de um documento deverá ser obrigado o upload de um ou mais arquivo PDF ou XML.

**Exemplo:**

Para uma Nota Fiscal, o usuário configura em seu nível de árvore como **Parâmetros para obrigatoriedade de arquivo**: 1 PDF e 1 XML.

Durante a Indexação da Nota Fiscal para este nível de árvore, a aplicação não irá permitir que o documento seja indexado se não houver pelo menos 1 arquivo com extensão PDF e 1 arquivo com extensão XML.

Essa funcionalidade, garante que documentos importantes sejam indexados com seus respectivos arquivos, quantos foram configurados e quantas extensões forem indicadas. Levando em consideração integrações com a API, um documento nunca será indexado com arquivos faltantes.

{% hint style="warning" %}
<mark style="color:orange;">Não há leitura do conteúdo do arquivo, apenas a indicação da extensão do arquivo.</mark>
{% endhint %}
