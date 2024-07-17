# 🟩 API

No menu API o cliente tem acesso a uma chave que será utilizada para gerenciamento e controle das requisições realizadas via API.&#x20;

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Unidade - Cliente:** Selecione neste campo o nome da unidade e cliente. Aqui são listados todos os clientes que possuem o serviço ArqAPI vigente no contrato.

Ao selecionar o campo, o botão "Gerar: Par de Chaves" é habilitado na tela.

**Chave 1:** Quando o cliente ainda não possui chave gerada o campo é apresentado em branco, quando o cliente já tem chave gerada é apresentada a chave 1 gerada automaticamente pelo sistema.

**Chave 2:** Quando o cliente ainda não possui chave gerada o campo é apresentado em branco, quando o cliente já tem chave gerada é apresentada a chave 2 gerada automaticamente pelo sistema.

{% hint style="danger" %}
<mark style="color:red;">Por</mark> <mark style="color:red;"></mark><mark style="color:red;">**padrão**</mark> <mark style="color:red;"></mark><mark style="color:red;">o sistema vai gerar sempre um</mark> <mark style="color:red;"></mark><mark style="color:red;">**"par" de chaves**</mark><mark style="color:red;">, então o cliente poderá utilizar</mark> <mark style="color:red;"></mark><mark style="color:red;">**uma ou outra**</mark> <mark style="color:red;"></mark><mark style="color:red;">ou em casos em que a integração ocorre com terceiros, o cliente utiliza uma e o parceiro outra.</mark>

<mark style="color:red;">Uma vez que a chave é gerada, ela deve ser incluída no HEADER das requisições para que estas sejam autorizadas.</mark>
{% endhint %}

