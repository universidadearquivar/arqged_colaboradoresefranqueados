# 📋 Lista

O objetivo do menu Lista é criar listas de pessoas ou de empresas dentro do sistema para posteriormente associar campos de formulários a essas listas, facilitando a indexação dentro do sistema. &#x20;

Ao se criar uma lista associa-se a ela uma série de campos. Na criação da árvore documental pode-se determinar que em um tipo documental será utilizada uma lista e todas as pessoas ou empresas que estejam nessa lista terão os campos automaticamente preenchidos nos formulários dos fluxos de trabalho. &#x20;

{% hint style="info" %}
<mark style="color:blue;">Em uma árvore documental de uma empresa, existe o departamento de RH e o tipo documental Folha de Ponto. A Folha de Ponto é composta pela lista “Funcionários”.</mark> &#x20;

<mark style="color:blue;">A lista “Funcionários” possui os campos “Matrícula”, “Nome do Funcionário” e “Cargo”. Isso significa que ao preencher durante um fluxo de trabalho, ao preencher o formulário de uma folha de ponto será necessário informar apenas um dos campos da lista “Funcionários”. Ao inserir a matrícula, por exemplo, os outros dois campos serão preenchidos automaticamente com o nome e o cargo do funcionário proprietário da matrícula informada.</mark>
{% endhint %}

{% hint style="warning" %}
<mark style="color:orange;">**Na lista devem ser cadastrados campos que não variam, ou seja, que não vão ser alterados independente do documento, como data de nascimento, nome, matrícula, CNPJ, admissão, demissão etc. Campos variáveis devem ser criados como customizados.**</mark>
{% endhint %}

Existem dois tipos de lista no sistema: &#x20;

* **Consolidação:** A lista de Consolidação permite a inclusão de informações durante a indexação, ou seja, se no momento de cadastrar um documento composto por uma lista eu informar um dado de pessoa ou empresa ainda não informado anteriormente, o sistema permitirá que eu insira os dados manualmente naquele momento e a partir daí, nas próximas vezes que utilizar um documento com essa mesma lista, ele extrairá as informações automaticamente. A lista de Consolidação é utilizada para auditoria dentro do sistema &#x20;
* **Auto Complete:** Na lista Auto Complete só é permitido incluir informações antes da indexação, como itens de lista. A lista de Auto Complete não pode ser utilizada para auditoria. &#x20;

O menu Lista é composto pelos seguintes submenus:

<table data-card-size="large" data-view="cards"><thead><tr><th align="center"></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td align="center"><mark style="color:green;"><strong>Criar Listas</strong></mark></td><td><a href="criar-listas.md">criar-listas.md</a></td></tr><tr><td align="center"><mark style="color:green;"><strong>Configurar</strong></mark></td><td><a href="configurar.md">configurar.md</a></td></tr></tbody></table>
