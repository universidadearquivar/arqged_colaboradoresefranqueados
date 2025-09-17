# ▫️ Abril | 2025

<details>

<summary>17/04 - Autenticação multifator (MFA)</summary>

**MFA**&#x20;

O "[**Login com MFA**](abril-or-2025.md#login-com-mfa-autenticacao-multifator)" refere-se ao acesso por meio de autenticação multifator. A sigla MFA (do inglês _Multifactor Authentication_) representa um método de segurança que exige que o usuário forneça duas ou mais formas de autenticação para acessar uma aplicação.

Essa abordagem adiciona uma camada extra de proteção, tornando o acesso não autorizado mais difícil, mesmo que a senha do usuário seja comprometida.

<div align="left"><figure><img src="../.gitbook/assets/image (343).png" alt="" width="179"><figcaption></figcaption></figure></div>

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

&#x20;**Usuários com acesso via SSO**

Usuários de clientes que utilizam **SSO (Single Sign-On)** para acessar o ArqGED **não utilizarão o MFA do ArqGED**, uma vez que a autenticação com múltiplos fatores estará configurada e gerenciada diretamente pelo SSO do cliente.

</details>
