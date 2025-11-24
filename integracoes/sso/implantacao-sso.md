# 🛠️ Implantação SSO

## Configurações no ArqGED

Acesse a URL do ArqGED e clique na opção "Entrar com SSO".

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Será apresentada uma nova tela para inclusão do código do AD (Active Directory) que é o código que identifica o Cliente ArqGED nas configurações de acesso do AD do cliente.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Se neste momento for informado um código incorreto, a aplicação exibirá uma mensagem de alerta ao usuário <mark style="color:red;">**"Erro ao autenticar: \[código] inválido."**</mark>

<figure><img src="../../.gitbook/assets/image (149).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Sendo informado o código correto, a aplicação identificará o Cliente e sua respectiva configuração para chamar seu IdP.

O ArqGED irá chamar o IdP do Cliente com um ID que identifica a aplicação ArqGED na ferramenta dele.

Abaixo está um exemplo de integração com o Azure AD. Neste caso, após informar o código que identifica o cliente e clicar “Entrar”, é exibido no browser do Cliente a página de autenticação da Microsoft.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

## Usuário autenticado no Idp do Cliente

### Quando o usuário <mark style="color:red;">não existe</mark> no ArqGED

Se o usuário não existir no ArqGED, esta autenticação no IdP irá enviar os dados do usuário para o ArqGED.

O ArqGED irá criar o usuário vinculado ao cliente, porém com o status “**Bloqueado**” e sem a parametrização das permissões de árvore documental e perfil de usuário e será apresentada ao usuário uma mensagem de orientação para a devida liberação dos acessos.

Na mensagem existem os dados: **Email, Nome e Telefone.** Estas informações poderão ser personalizadas por Cliente, de forma que o usuário que acabou de ser criado no ArqGED via IdP, saiba a quem procurar para solicitar a atribuição de permissões de árvore documental e perfis de acesso.

<figure><img src="../../.gitbook/assets/image (150).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Após o desbloqueio do usuário e atribuição de árvore documental juntamente com o perfil de acesso, na próxima tentativa de login, o usuário será autenticado no ArqGED.

### Quando o usuário <mark style="color:green;">já existe</mark> no ArqGED

Quando no primeiro acesso o usuário já estiver “Ativo” no ArqGED e com as permissões de acesso atribuídas, após a autenticação com sucesso no IdP do Cliente, ele será direcionado já autenticado e autorizado no ArqGED.

<figure><img src="../../.gitbook/assets/image (151).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">Se o usuário for</mark> <mark style="color:orange;">**bloqueado ou inativado no ArqGED**</mark> <mark style="color:orange;">e tentar acessar a aplicação, ele sempre será direcionado para a tela com a mensagem de "Autorização no ArqGED".</mark>

<img src="../../.gitbook/assets/image (154).png" alt="" data-size="original">

<mark style="color:orange;">Se o usuário for</mark> <mark style="color:orange;">**bloqueado ou inativado no IdP do Cliente**</mark><mark style="color:orange;">, ele não conseguirá avançar, a aplicação ficará tentando autenticação no IdP, sem sucesso.</mark>
{% endhint %}

***

## Pré-Requisitos do SSO

Antes de ir para os passos de configuração, o cliente **precisa ter um IdP que funcione com o protocolo SAML 2.0 de autenticação.**

### Passos para se configurar o SSO

O cliente precisa passar pelos tópicos abaixo para iniciar o processo de configuração do SSO:

1. **Incluir no seu IdP os dados**
   1. Identifier (Entity ID): https://ssosp.arquivar.com
   2. Reply URL (Assertion Consumer Service URL): https://arqged.arquivar.com/Account/LoginViaSSO
2. **Enviar para a Arquivar os dados**
   1. IdPMetadataXML
   2. ClaimNomeUsuario (enviar nome completo)
   3. ClaimEmail
3. **Enviar para a Arquivar os dados de contato do responsável por atribuir as permissões dentro do ArqGED**
   1. Email
   2. Nome
   3. Telefone

Após receber as informações listadas anteriormente, a Arquivar irá:

1. Fazer as configurações no ArqGED com os dados enviados pela empresa;
2. Enviar o código SSO que será usado no início do processo de autenticação.

{% hint style="danger" %}
<mark style="color:red;">Para quem estiver usando o SSO</mark>

<mark style="color:red;">É importante saber que por questões de segurança e para garantir que um usuário criado via processo de SSO somente consiga acessar desta forma, as funções abaixo foram bloqueadas para este tipo de usuário:</mark>

<mark style="color:red;">• Usuários criados via SSO não podem executar a ação de alterar senha através do link “Esqueceu a senha?”.</mark>

<mark style="color:red;">• Usuários criados via SSO, não poderão ser autenticados via tela de login do ArqGED (com usuário e senha na tela de login).</mark>

<mark style="color:red;">• Usuários criados via SSO, não poderão incluir outros usuários no ArqGED.</mark>

<mark style="color:red;">• Usuários criados via SSO, não poderão ser autenticados via API.</mark>
{% endhint %}
