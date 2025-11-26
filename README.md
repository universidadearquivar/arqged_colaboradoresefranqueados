# 🟢 Página inicial

{% embed url="https://app.heygen.com/videos/da6ffe6e098849e29676a1a12e419098" %}

Bem-vindo(a) ao guia do sistema ArqGED da Arquivar!

O software ArqGED é um BPM (Business Process Management), desenvolvido pela Arquivar que **possibilita a gestão de processos, a digitalização, o gerenciamento e o armazenamento de documentos** importantes em um ambiente virtual seguro, acessível apenas por usuários autorizados.

Neste guia  você encontrará diversos conteúdos que te ajudarão a utilizar nossa ferramenta da melhor forma. Utilize a navegação à esquerda para conhecer as funcionalidades de cada menu do software ArqGED.



***

## Autenticação – MFA

### Login com MFA (Autenticação Multifator)

O "Login com MFA" refere-se ao acesso por meio de autenticação multifator. A sigla MFA (do inglês _Multifactor Authentication_) representa um método de segurança que exige que o usuário forneça duas ou mais formas de autenticação para acessar uma aplicação.

Essa abordagem adiciona uma camada extra de proteção, tornando o acesso não autorizado mais difícil, mesmo que a senha do usuário seja comprometida.

**Como funciona no ArqGED**

No ArqGED, o processo de login com MFA funciona da seguinte forma:

**1.** O usuário informa seu **nome de usuário e senha.**

**2.** Em seguida, deverá informar um **código de verificação.**

Esse código é **dinâmico** e muda a cada tentativa de login.

O código pode ser obtido de duas maneiras:

**Via Aplicativo Autenticador**                                                                                                                                                 O usuário pode escolher entre diversos aplicativos gratuitos disponíveis no mercado, como:

* Google Authenticator
* Microsoft Authenticator

Para utilizar essa opção, é necessário instalar o aplicativo escolhido no celular e seguir as instruções de configuração no ArqGED.

**Via E-mail**                                                                                                                                                                                   O código de verificação será enviado para o e-mail cadastrado no usuário. Para utilizar essa opção, é preciso validar previamente o e-mail seguindo o fluxo indicado no ArqGED.

**Recomendação importante**

É altamente recomendável que o usuário **configure as duas opções de MFA** (Aplicativo Autenticador e E-mail). Dessa forma, caso esteja sem acesso ao celular, poderá utilizar o e-mail para receber o código — e vice-versa.

&#x20;**Usuários com acesso via SSO**

Usuários de clientes que utilizam **SSO (Single Sign-On)** para acessar o ArqGED **não utilizarão o MFA do ArqGED**, uma vez que a autenticação com múltiplos fatores estará configurada e gerenciada diretamente pelo SSO do cliente.

### Impor Autenticação MFA

A autenticação MFA será **obrigatória para todos os usuários de Unidade.**&#x20;Dessa forma, ao acessarem o ArqGED pela primeira vez após a publicação dessa funcionalidade, esses usuários serão direcionados automaticamente para o fluxo de configuração do MFA. Será necessário configurar **pelo menos uma opção de autenticação** antes de terem acesso completo ao ArqGED.

Para os **usuários do Cliente**, o uso do MFA será **opcional por padrão**.

Caso o cliente deseje obrigar o uso de MFA solicite a Arquivar a imposição desta configuração para seus usuários.\
No entanto, caso o Cliente deseje tornar o uso do MFA obrigatório, será necessário marcar a opção **"Impor autenticação MFA"** no cadastro da conta do Cliente, conforme ilustrado na imagem abaixo:

<figure><img src=".gitbook/assets/image (257).png" alt=""><figcaption></figcaption></figure>

### Configuração do MFA: via Login

O primeiro acesso dos usuários de **Unidade ou Cliente** com a configuração de **"Impor autenticação MFA"**, seguirá o fluxo abaixo:

**a)** Na tela inicial, o usuário deve inserir seu **nome de usuário, senha, captcha e clicar no botão “Entrar”**, conforme ilustrado abaixo:

<figure><img src=".gitbook/assets/image (256).png" alt="" width="313"><figcaption></figcaption></figure>

Ao clicar no botão **“Entrar”**, o sistema redirecionará automaticamente para uma nova tela com instruções passo a passo para configuração da autenticação.

**b)** Nesta tela será exibido:

* &#x20;O nome do usuário autenticado.
* A informação de que o MFA foi imposto pela organização.
* Os passos necessários para configurar a autenticação via aplicativo ou e-mail.

<div align="left"><figure><img src=".gitbook/assets/image (201).png" alt="" width="326"><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/image (202).png" alt="" width="322"><figcaption></figcaption></figure></div>

Enquanto o usuário não possuir nenhuma configuração, como primeiro passo, o usuário poderá escolher qual deseja configurar primeiro:

* Aplicativo Autenticador
* E-mail cadastrado no ArqGED

**c)** Ao escolher a opção **“Aplicativo Autenticador”**, a tela exibe os passos que deverão ser seguidos, conforme abaixo:

<figure><img src=".gitbook/assets/image (203).png" alt="" width="493"><figcaption></figcaption></figure>

* Para iniciar, deve-se baixar um aplicativo autenticador para o celular;
* Abrir o aplicativo instalado e ler o QRCode que está sendo exibido na tela do ArqGED.

**Nota:** Consultar ao final deste documento “Anexo 1 – Como usar o Microsoft Authenticator” e “Anexo 2 – Como usar o Google Authenticator”.

* Após a leitura do QRCode, o aplicativo autenticador exibirá um código na tela. Este código deve ser inserido no passo 4, conforme indicado abaixo:

<figure><img src=".gitbook/assets/image (204).png" alt="" width="479"><figcaption></figcaption></figure>

* Com o código de verificação inserido no campo conforme a imagem, deve-se clicar no botão **“Avançar”**. Neste momento o usuário será direcionado para a tela com a mensagem sucesso.
* Quando o usuário terminar de configurar o “Aplicativo Autenticador” e ainda faltar a configuração do “E-mail”, a tela além de exibir a mensagem de sucesso, exibira os botões “Entrar no ArqGED” ou “Configurar Outra Opção”. &#x20;

<figure><img src=".gitbook/assets/image (205).png" alt="" width="447"><figcaption></figcaption></figure>

Se o usuário escolher “Configurar outra opção”, ele entrará no fluxo de configuração do e-mail. Se ele escolher “Entrar no ArqGED”, ele será autenticado na aplicação, mas em seu próximo login, será lembrado de configurar o e-mail.

* Quando o usuário terminar de configurar o “Aplicativo Autenticador” e o “E-mail” já estiver configurado também, a tela a ser exibida terá somente a mensagem de sucesso e o botão “Entrar no ArqGED”.

<figure><img src=".gitbook/assets/image (206).png" alt="" width="443"><figcaption></figcaption></figure>

**d)** Ao escolher a opção **“E-mail cadastrado no ArqGED”**, a tela exibe os passos que deverão ser seguidos, conforme abaixo:

<figure><img src=".gitbook/assets/image (207).png" alt="" width="495"><figcaption></figcaption></figure>

* Deve-se conferir se o e-mail que está sendo exibido na tela está correto. Se estiver correto o usuário poderá prosseguir com a configuração, se não estiver correto, deve-se entrar em contato com o usuário Administrador para corrigir este e-mail.
* Estando o e-mail correto, o usuário deverá clicar em **“Enviar código”**. Neste momento a aplicação enviará um código de verificação para o e-mail do usuário através do remente [autenticacao@arquivar.com](mailto:autenticacao@arquivar.com), com o assunto **Código segurança MFA**.

<figure><img src=".gitbook/assets/image (208).png" alt="" width="503"><figcaption></figcaption></figure>

* Este código deverá ser inserido no passo 3, conforme a imagem a seguir.

<figure><img src=".gitbook/assets/image (209).png" alt=""><figcaption></figcaption></figure>

* Com o código de verificação inserido no campo conforme a imagem, ao clicar no botão “Avançar”, o usuário será direcionado para a tela com a mensagem sucesso.
* Quando o usuário terminar de configurar o “E-mail” e ainda faltar a configuração do “Aplicativo Autenticador”, a tela além de exibir a mensagem de sucesso, exibira os botões “Entrar no ArqGED” ou “Configurar Outra Opção”. &#x20;
* Se o usuário escolher “Configurar outra opção”, ele entrará no fluxo de configuração do Aplicativo Autenticador. Se ele escolher “Entrar no ArqGED”, ele será autenticado na aplicação, mas em seu próximo login, será lembrado de configurar o Aplicativo Autenticador.

<figure><img src=".gitbook/assets/image (210).png" alt="" width="490"><figcaption></figcaption></figure>

* Quando o usuário terminar de configurar o “Email” e o “Aplicativo Autenticador” já estiver configurado também, a tela a ser exibida terá somente a mensagem de sucesso e o botão “Entrar no ArqGED”.

<figure><img src=".gitbook/assets/image (211).png" alt="" width="451"><figcaption></figcaption></figure>

O fluxo de configuração via Login conforme descrito, somente será exibido aos usuários que ainda não possuem configuração de MFA e que atendam aos requisitos abaixo:

* Usuários de Unidade; ou
* Usuários dos Cliente que em seu cadastro possuem a flag “Impor Autenticação MFA” marcada.

### Configuração do MFA: Acessar o menu via ArqGED

Todos os usuários do ArqGED, exceto os que utilizam SSO para autenticar, poderão acessar as configurações de MFA, pelo menu abaixo:

<figure><img src=".gitbook/assets/image (4) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Ao acessar a tela de “MFA – Autenticação Multifator”, serão exibidas as duas opções de configuração: Aplicativo Autenticador e Email.

As possíveis telas são:

**a) Quando nenhuma opção estiver configurada ainda:**

A tela abaixo será exibida para usuários de Clientes que não possuem configuração de MFA imposta ou para usuários que acabaram de excluir a configuração de aplicativo ou teve seu e-mail alterado.

Quando nenhuma das opções estiverem configuradas, o usuário poderá realizar as duas configurações usando o link “Configurar”

<figure><img src=".gitbook/assets/image (213).png" alt=""><figcaption></figcaption></figure>

**b) Quando todas as opções estiverem configuradas:**

Quando as duas opções de configuração estiverem concluídas no ArqGED, o usuário poderá escolher qual será o seu padrão de autenticação, ou seja, qual o ArqGED irá solicitar no ato do login.

A escolha da opção padrão, deve ser feita pelo link “Definir como padrão”.

<figure><img src=".gitbook/assets/image (214).png" alt=""><figcaption></figcaption></figure>

**Nota:** Observe que na configuração de **“Aplicativo Autenticador”** existe a opção **“Excluir”**. O usuário deve usar este recurso quando quiser trocar de celular, então primeiro ele deve **“Excluir”** a configuração anterior no ArqGED, e seguir novamente os passos de configuração no novo celular.

Observe também que para o e-mail não existe a opção de excluir, mas sempre que o e-mail do usuário for alterado, caso ele esteja sendo usado como opção de MFA, a sua configuração será excluída e o usuário precisará passar pelo processo de validação do e-mail novamente antes de usar este novo e-mail como opção de MFA.

**c) Quando somente aplicativo configurado:**

Quando o usuário possuir somente o **“Aplicativo Configurado”**, esta será a sua opção padrão para autenticação.

Neste caso, a opção de e-mail será exibida com pendência de configuração, e um botão **“Configurar”** estará disponível para o usuário concluir este processo.

<figure><img src=".gitbook/assets/image (215).png" alt=""><figcaption></figcaption></figure>

**Nota:** Observe que na configuração de “Aplicativo Autenticador” existe a opção “Excluir”. O usuário deve usar este recurso quando quiser trocar de celular, então primeiro ele deve “Excluir” a configuração anterior no ArqGED, e seguir novamente os passos de configuração no novo celular.

**d) Quando somente e-mail configurado:**

Quando o usuário possuir somente o **“E-mail”** configurado, esta será a sua opção padrão para autenticação.

Neste caso, a opção de Aplicativo será exibida com pendência de configuração, e um botão **“Configurar”** estará disponível para o usuário concluir este processo.

<figure><img src=".gitbook/assets/image (217).png" alt=""><figcaption></figcaption></figure>

**Nota:** Observe que para o e-mail não existe a opção de excluir, mas sempre que o e-mail do usuário for alterado, caso ele esteja sendo usado como opção de MFA, a sua configuração será excluída e o usuário precisará passar pelo processo de validação do e-mail novamente antes de usar este novo e-mail como opção de MFA.

### Configuração do MFA: Fluxo via ArqGED

Após autenticar no ArqGED, o usuário poderá acessar o menu **“MFA – Autenticação Multifator”**, conforme tela abaixo:

<figure><img src=".gitbook/assets/image (5) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

A aplicação irá exibir as duas opções disponíveis, conforme tela abaixo:

<figure><img src=".gitbook/assets/image (219).png" alt=""><figcaption></figcaption></figure>

Caso falte alguma para configurar, o usuário poderá seguir o fluxo de configuração conforme descrito a seguir:

**a) Fluxo de Configuração do Aplicativo**

Para iniciar o fluxo de configuração do aplicativo, o usuário deverá pressionar o link **“Configurar”** conforme mostra abaixo:

<figure><img src=".gitbook/assets/image (220).png" alt=""><figcaption></figcaption></figure>

Na sequência a aplicação exibirá a tela conforme abaixo, e o usuário deverá seguir as instruções desta tela para finalizar a configuração do aplicativo (Os passos são os mesmos descritos no tópico 3, letra C:

<figure><img src=".gitbook/assets/image (221).png" alt=""><figcaption></figcaption></figure>

Ao finalizar a configuração do aplicativo, a aplicação voltará para a tela abaixo, mostrando o aplicativo configurado:

<figure><img src=".gitbook/assets/image (222).png" alt=""><figcaption></figcaption></figure>

**b) Fluxo de Configuração do Email**

Para iniciar o fluxo de configuração do e-mail, o usuário deverá pressionar o link **“Configurar”** conforme mostra abaixo:

<figure><img src=".gitbook/assets/image (223).png" alt=""><figcaption></figcaption></figure>

Na sequência a aplicação exibirá a tela conforme abaixo, e o usuário deverá seguir as instruções desta tela para finalizar a configuração do aplicativo (Os passos são os mesmos descritos no tópico 3, letra D):

<figure><img src=".gitbook/assets/image (224).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (225).png" alt=""><figcaption></figcaption></figure>

Ao finalizar a configuração do e-mail, a aplicação voltará para a tela abaixo, mostrando o aplicativo configurado:

<figure><img src=".gitbook/assets/image (226).png" alt=""><figcaption></figcaption></figure>

### Fluxo de Login: Quando o usuário possuir somente uma configuração de MFA

Mesmo para os usuários com o uso de MFA obrigatório, ele poderá configurar somente uma opção e na sequência escolher **“Entrar no ArqGED”**, conforme vimos nas telas abaixo:

<figure><img src=".gitbook/assets/image (227).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (229).png" alt=""><figcaption></figcaption></figure>

Vimos também que um usuário de Cliente que não possui a configuração imposta, poderá optar por usar o MFA, fazendo a configuração do mesmo não no fluxo de login, mas dentro do ArqGED. E neste caso também será permitido configurar somente uma opção deixando a outra para configurar mais tarde.

&#x20;Desta forma, sempre que o usuário possuir somente uma opção de MFA configurada, assim que ele informar seu usuário, senha, captcha e clicar para **“Entrar”** na tela de login, ele será direcionado para uma das duas telas abaixo:

<figure><img src=".gitbook/assets/image (230).png" alt="" width="386"><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (231).png" alt="" width="335"><figcaption></figcaption></figure>

Nesta tela, o usuário poderá escolher entrar no ArqGED com o MFA já configurado, ou entrar no fluxo de configuração da outra opção de MFA faltante.

Sempre que o usuário já possuir o Aplicativo configurado, e via tela de login, entrar no fluxo de configuração do e-mail, a tela a ser exibida será a abaixo. Observe que no passo 1 desta tela, somente existe a opção de e-mail disponível e ela já se encontra marcada:

<figure><img src=".gitbook/assets/image (232).png" alt=""><figcaption></figcaption></figure>

Sempre que o usuário já possuir o E-mail configurado, e via tela de login, entrar no fluxo de configuração do aplicativo, a tela a ser exibida será a abaixo. Observe que no passo 1 somente existe a opção de aplicativo disponível e ela já se encontra marcada:

<figure><img src=".gitbook/assets/image (233).png" alt=""><figcaption></figcaption></figure>

Observe também que no rodapé destas duas telas possui a opção **“Voltar para tela anterior”**, isso é possível porque como o usuário já possui uma opção de MFA configurada, ele pode desistir do fluxo de configuração e voltar para a tela anterior e então decidir entrar no ArqGED.

### Fluxo de Login: Quando o usuário possuir as duas opções de configuração de MFA

Quando o usuário já estiver com as duas opções de MFA configurada, o fluxo de login será conforme abaixo:

**a)** Na tela inicial, o usuário deve inserir seu **nome de usuário, senha, captcha e clicar no botão “Entrar”**, conforme ilustrado abaixo:

<figure><img src=".gitbook/assets/image (234).png" alt=""><figcaption></figcaption></figure>

**b)** Assim que o usuário clicar no botão **“Entrar”**, a aplicação seguirá para a tela onde se informa o código MFA. Se a opção padrão do usuário for o **“Aplicativo Autenticador”** então será exibida a tela abaixo:

<figure><img src=".gitbook/assets/image (235).png" alt=""><figcaption></figcaption></figure>

Se a opção padrão do usuário for do **“Email”** então será exibida a tela abaixo:

<figure><img src=".gitbook/assets/image (236).png" alt=""><figcaption></figcaption></figure>

Observe que quando o usuário possuir as duas configurações de MFA, mesmo exibindo a sua opção padrão como primeira opção, a aplicação o permitirá usar a outra opção, clicando em **“Informar o código do aplicativo configurado”** ou **“Enviar código para o e-mail”**.

<figure><img src=".gitbook/assets/image (237).png" alt="" width="312"><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (238).png" alt="" width="335"><figcaption></figcaption></figure>

**Nota:** A opção de MFA default (padrão) será a que foi configurada primeiro pelo usuário. Mas o usuário poderá trocar a sua preferência após logar no ArqGED, conforme no tópico 4, letra b.

**c)** Se o usuário for usar o aplicativo, então ele deve abrir o aplicativo no celular e o código que estiver sendo exibido para o ArqGED, o usuário deve informar no campo da tela abaixo e clicar no botão **“Entrar”.**

<figure><img src=".gitbook/assets/image (239).png" alt=""><figcaption></figcaption></figure>

**d)** Se o usuário for usar o e-mail, então ele deve abrir o seu e-mail e identificar a mensagem enviada pelo remetente [autenticacao@arquivar.com](mailto:autenticacao@arquivar.com), com o assunto Código segurança MFA.

<figure><img src=".gitbook/assets/image (240).png" alt="" width="511"><figcaption></figcaption></figure>

O código desta mensagem deve ser inserido na tela abaixo:

<figure><img src=".gitbook/assets/image (241).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Importante: Uma vez autenticado com o uso do MFA com sucesso, a aplicação irá solicitar novamente o MFA naquele dia somente se:**</mark>

* <mark style="color:orange;">**O usuário clicar no botão “Sair” do ArqGED, no canto superior direito da tela.**</mark>
* <mark style="color:orange;">**O usuário usar outro computador para acessar o ArqGED.**</mark>
* <mark style="color:orange;">**O usuário no mesmo computador usar outro navegador para acessar o ArqGED.**</mark>
{% endhint %}

### Anexo I: Como usar o Microsoft Authenticator

<div align="left"><figure><img src=".gitbook/assets/image (242).png" alt="" width="195"><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/image (243).png" alt="" width="193"><figcaption></figcaption></figure></div>

Clicar no botão **“Adicionar conta”** irá abrir outra tela. Nesta tela deve ser escolhido a opção **“Outro (Google, Facebook, etc...)”**. A câmera do celular será aberta para digitalização do QR code na tela.

<div align="left"><figure><img src=".gitbook/assets/image (244).png" alt="" width="288"><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/image (245).png" alt="" width="233"><figcaption></figcaption></figure></div>

A leitura do QR code, irá gerar um código de verificação na tela que deve ser inserido no passo 4, conforme explicado.

### Anexo I: Como usar o Google Authenticator

Tela inicial do aplicativo. Não há necessidade de realizar login para utilização.

<div align="left"><figure><img src=".gitbook/assets/image (246).png" alt="" width="189"><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/image (247).png" alt="" width="194"><figcaption></figcaption></figure></div>

Clicar no botão **“Adicionar um código”** irá exibir uma tela para leitura do QrCorde ou a inserção da chave.

&#x20;Utilizar a opção **“Ler QR code”** irá abrir a câmera do celular, que deve ser direcionada para o código na tela do ArqGED.

<div align="left"><figure><img src=".gitbook/assets/image (248).png" alt="" width="208"><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/image (249).png" alt="" width="201"><figcaption></figcaption></figure></div>

Após a leitura do QR Code, na tela do aplicativo será exibido um código de verificação. Este código deve inserido no passo 4, conforme explicado.

## Links para Aplicativos Authenticadores

<div align="left"><figure><img src=".gitbook/assets/image (250).png" alt="" width="122"><figcaption><p>Google Authenticator</p></figcaption></figure></div>

{% embed url="https://play.google.com/store/search?q=google+authenticator&c=apps&hl=pt_BR" %}

{% embed url="https://apps.apple.com/br/app/google-authenticator/id388497605" %}

<div align="left"><figure><img src=".gitbook/assets/image (251).png" alt="" width="162"><figcaption><p>Microsoft Authenticator</p></figcaption></figure></div>

{% embed url="https://play.google.com/store/search?q=microsoft%20authenticator&c=apps&hl=pt_BR" %}

{% embed url="https://apps.apple.com/br/app/microsoft-authenticator/id983156458" %}

<div align="left"><figure><img src=".gitbook/assets/image (252).png" alt="" width="113"><figcaption><p>Twilio Authy Authenticator</p></figcaption></figure></div>

{% embed url="https://play.google.com/store/search?q=authy%20authenticator&c=apps&hl=pt_BR" %}

{% embed url="https://apps.apple.com/br/app/twilio-authy/id494168017" %}
