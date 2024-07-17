# 🟩 API

No menu API o cliente tem acesso a uma chave que será utilizada para gerenciamento e controle das requisições realizadas via API.&#x20;

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Unidade - Cliente:** Selecione neste campo o nome da unidade e cliente. Aqui são listados todos os clientes que possuem o serviço ArqAPI vigente no contrato.

Ao selecionar o campo, o botão "Gerar: Par de Chaves" é habilitado na tela.

**Chave 1:** Quando o cliente ainda não possui chave gerada o campo é apresentado em branco, quando o cliente já tem chave gerada é apresentada a chave 1 gerada automaticamente pelo sistema.

**Chave 2:** Quando o cliente ainda não possui chave gerada o campo é apresentado em branco, quando o cliente já tem chave gerada é apresentada a chave 2 gerada automaticamente pelo sistema.

{% hint style="info" %}
<mark style="color:blue;">Por</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**padrão**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">o sistema vai gerar sempre um</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**"par" de chaves**</mark><mark style="color:blue;">, então o cliente poderá utilizar</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**uma ou outra**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">ou em casos em que a integração ocorre com terceiros, o cliente utiliza uma e o parceiro outra.</mark>

<mark style="color:blue;">Uma vez que a chave é gerada, ela deve ser incluída no HEADER das requisições para que estas sejam autorizadas.</mark>
{% endhint %}

Ao clicar em Gerar: Par de Chaves, é exibida uma mensagem informativa na tela.

<figure><img src="../.gitbook/assets/image (44).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>



{% hint style="danger" %}
<mark style="color:red;">Se após regerar as chaves, o usuário não atualizá-las nos parâmetros de pesquisa da integração  já existente, as chamadas na API do ArqGED deixarão de funcionar!</mark>
{% endhint %}

Clicando no ícone "Visualizar" para mostrar ou ocultar as chaves.

<figure><img src="../.gitbook/assets/image (45).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Para **regerar o par de chaves**, utilize o botão **"Gerar: Par de Chaves".** Para **regerar apenas uma das chaves, utilize o** ícone de **"Regerar Chave"** considerando a chave 1 ou a 2.

<figure><img src="../.gitbook/assets/image (46).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

