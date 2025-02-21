# 🔌 SSO

_Single sign-on_ (SSO) ou, em português, “**login único**” é uma tecnologia de autenticação que permite que um usuário use um único login — seu e-mail e senha, por exemplo — para acessar vários aplicativos.

Com o SSO, o usuário acessa várias telas de login unificadas em uma só, permitindo a inserção das credenciais de maneira conjunta, o que simplifica o processo de autenticação.

Um dos grandes diferenciais do SSO é que, hoje em dia, usam-se muitos serviços digitais e diferentes softwares que requerem login e senha.&#x20;

O ArqGED está preparado para usar este modelo de autenticação e para isso, é necessário realizar algumas configurações dentro da aplicação.

## Configurações no ArqGED

Acesse a URL do ArqGED e clique na opção "Entrar com SSO".

<figure><img src="../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Será apresentada uma nova tela para inclusão do código do AD (Active Directory) que é o código que identifica o Cliente ArqGED nas configurações de acesso do AD do cliente.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Se neste momento for informado um código incorreto, a aplicação exibirá uma mensagem de alerta ao usuário <mark style="color:red;">**"Erro ao autenticar: \[código] inválido."**</mark>

<figure><img src="../.gitbook/assets/image (149).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Sendo informado o código correto, a aplicação identificará o Cliente e sua respectiva configuração para chamar seu IdP.&#x20;

O ArqGED irá chamar o IdP do Cliente com um ID que identifica a aplicação ArqGED na ferramenta dele.&#x20;

Abaixo está um exemplo de integração com o Azure AD. Neste caso, após informar o código que identifica o cliente e clicar “Entrar”, é exibido no browser do Cliente a página de autenticação da Microsoft.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

## Usuário autenticado no Idp do Cliente

### Quando o usuário <mark style="color:red;">não</mark> existe no ArqGED

Se o usuário não existir no ArqGED, esta autenticação no IdP irá enviar os dados do usuário para o ArqGED.&#x20;

O ArqGED irá criar o usuário vinculado ao cliente, porém com o status “**Bloqueado**” e sem a parametrização das permissões de árvore documental e perfil de usuário e será apresentada ao usuário uma mensagem de orientação para a devida liberação dos acessos.

<figure><img src="../.gitbook/assets/image (150).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>
