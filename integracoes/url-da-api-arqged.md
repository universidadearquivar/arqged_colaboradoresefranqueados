# 🟩 URL da API ArqGED

{% embed url="https://app.heygen.com/videos/ffc1e32e582e4a25ade420a6c6e7856b" %}

## Documentação: [https://developers.arquivar.com/](https://developers.arquivar.com)

Para visualizar a documentação online de API do ArqGED, acesse: [https://developers.arquivar.com/](https://developers.arquivar.com)

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Ao acessar a URL da documentação, é exibida a API disponível, ao clicar os dados são listados na tela.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

No canto esquerdo da tela é exibida a lista dos métodos disponíveis para a API.

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Clicando no método, é exibido do lado direito da tela o seu detalhamento.

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Search operations:** Utilize para buscar um método da API selecionada na tela.

**Group by tag:** Utilize para agrupar os métodos da API selecionada.

**Try it:** Utilize para testar o método.

Clicando na opção "Try it", é aberto no canto direito da tela os campos de parâmentros e headers para preenchimento e teste.

Para usar os métodos, primeiramente será necessário gerar um token de autenticação em [https://api-rest.arquivar.com/v1/api/Autenticacao/Login](https://api-rest.arquivar.com/v1/api/Autenticacao/Login). No método autenticação são informados a “SubscriptionKey” no “Headers” e os dados do Usuário no “Body”, conforme print abaixo:

<figure><img src="../.gitbook/assets/image (81).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Com o token retornado pelo método anterior, será possível usar os outros métodos. Então neste caso, na área do “Headers” precisam ser enviados a “[SubscriptionKey](../administracao/api.md#subscriptionkey-chave-de-acesso-ou-chave-de-api)” e token de autenticação no formato “Baerer Token” no campo “Authorization”:

<figure><img src="../.gitbook/assets/image (80).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>
