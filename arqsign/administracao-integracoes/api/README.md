# ▫️ API

No menu API o cliente tem acesso as chaves necessárias para o gerenciamento e controle das requisições realizadas via API de integração.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FdYph317G5VuPG3MqxhJ1%252Fimage.png%3Falt%3Dmedia%26token%3D8b66187f-d74c-4b78-8ccc-941fca13cee4&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=908a8b1e&#x26;sv=2" alt=""><figcaption></figcaption></figure>

## **AppKey** <a href="#appkey" id="appkey"></a>

Para realizar a integração da plataforma a outras ferramentas via API é necessária uma Chave de Acesso, que o usuário pode obter clicando em “Gerar Chave”. A chave gerada será apresentada no campo “API AppKey”.

{% hint style="danger" %}
**Sempre que gerada uma nova chave de acesso, todas as integrações feitas utilizando a chave anterior serão desconfiguradas. Sugerimos cautela ao criar novas chaves de acesso.**
{% endhint %}

## **SubscriptionKey** <a href="#subscriptionkey" id="subscriptionkey"></a>

Trata-se de chaves de acesso, criadas para trazer mais segurança na troca de informações entre plataformas externas e a ArqSign.

**Chave 1:** Quando o cliente ainda não possui chave gerada o campo é apresentado em branco, quando o cliente já tem chave gerada é apresentada a chave 1 que foi gerada automaticamente pelo sistema.

**Chave 2:** Quando o cliente ainda não possui chave gerada o campo é apresentado em branco, quando o cliente já tem chave gerada é apresentada a chave 2 que foi gerada automaticamente pelo sistema.

Por **padrão** o sistema vai gerar sempre um **"par"** de **chaves**, então o cliente poderá utilizar **uma ou outra** ou **poderão ser usadas de forma rotacionada**, ou seja, a cada chamada o usuário poderá usar uma, ou ainda em casos em que a integração ocorre com terceiros, **o cliente utiliza uma e o terceiro a outra**.

Uma vez que a chave é gerada, ela deve ser incluída no HEADER das requisições para que estas sejam autorizadas.

Ao clicar em "Gerar Par de Chaves", é exibida uma mensagem na tela de validação da ação.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FJOnyE7IpLWICSY1of1vG%252Fimage.png%3Falt%3Dmedia%26token%3D83334013-480e-402d-b632-3419ab637541&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=269a99bc&#x26;sv=2" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
Se após regerar as chaves, o usuário não atualizá-las nos parâmetros de pesquisa da integração já existente, as chamadas na API da ArqSign deixarão de funcionar
{% endhint %}

Para **regerar o par de chaves**, utilize o botão **"Gerar Par de Chaves".** Para **regerar apenas uma das chaves, utilize o** ícone de **"Regerar Chave"** considerando a chave 1 ou a 2.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252F7szKeQUSnxMCC4vL7bjH%252Fimage.png%3Falt%3Dmedia%26token%3D618f8547-1f76-49ed-9e76-b51d27844b6d&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=6f5fb749&#x26;sv=2" alt=""><figcaption></figcaption></figure>

## Como passar a AppKey e a SubscriptionKey <a href="#como-passar-a-appkey-e-a-subscriptionkey" id="como-passar-a-appkey-e-a-subscriptionkey"></a>

Considerando a rota: [https://api-rest.arqsign.com/](https://api-rest.arqsign.com/), é necessário enviar no “Headers” além da “AppKey” a “SubscriptionKey” conforme figura abaixo:

Clique na imagem para ampliar.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FuS5GZtCBZRTymRLprRLt%252Fimage.png%3Falt%3Dmedia%26token%3Dfbef54b7-4c5a-40a4-a655-35910ac7ac75&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=6db91377&#x26;sv=2" alt=""><figcaption></figcaption></figure>

***

## Serviços de Integração ArqSign <a href="#servicos-de-integracao-arqsign" id="servicos-de-integracao-arqsign"></a>

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252F3O6paoSUchBxdiKrtbup%252Fimage.png%3Falt%3Dmedia%26token%3Da6e59dd1-c9b8-4d4c-bb17-eadb4a019fd2&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=9946a6a0&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Ao clicar neste link, a aplicação irá abrir a página [**developers.arqsign.com**](https://developers.arqsign.com/?_ga=2.164255991.919308982.1733860166-872117669.1732909328) com os métodos disponíveis até o momento.

***

## Documentação API <a href="#documentacao-api" id="documentacao-api"></a>

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252Fr2P7HLxsy1RIl2Savdo8%252Fimage.png%3Falt%3Dmedia%26token%3Db0fa4c43-0e2a-4e34-8190-b5a2e2582236&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=6e49f1e9&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Ao clicar neste link, a aplicação irá abrir a página [**de detalhamento da API.**](https://manual.arquivar.com/guia-do-cliente/arqsign/administracao-integracoes)

***

## Download lista de Id's usuários <a href="#download-lista-de-ids-usuarios" id="download-lista-de-ids-usuarios"></a>

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252F5S590QwqPgYRx3eDV32J%252Fimage.png%3Falt%3Dmedia%26token%3D86a09c93-03e7-4d7c-9636-21b1e5e1fbe7&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=84c3b32b&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Ao clicar neste link a aplicação irá fazer o download de um arquivo .csv com a lista de todos os usuários ativos na conta e seu respectivo ID.

{% hint style="success" %}
A busca pelos usuários ativos da conta também pode ser realizada por API, para mais informações acesse o detalhamento do método: [POST/api/v1/usuarios/buscar-usuarios](https://manual.arquivar.com/guia-do-cliente/arqsign/administracao-integracoes/api/metodos-disponiveis-na-api/3.-usuarios/3.1.post-api-v1-usuarios-buscar-usuarios)
{% endhint %}

***

## Download lista de Id's pastas <a href="#download-lista-de-ids-pastas" id="download-lista-de-ids-pastas"></a>

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FZVAFMSmfyqMX9f3eMkdK%252Fimage.png%3Falt%3Dmedia%26token%3D72c5c358-3a0d-428e-9131-a7855e574df8&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=b9179968&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Ao clicar neste link a aplicação irá fazer o download de um arquivo .csv com a lista de todas as pastas não excluídas da conta e seu respectivo ID.

{% hint style="success" %}
A busca pelas pastas não excluídas da conta também pode ser realizada por API, para mais informações acesse o detalhamento do método: [POST/api/v1/diretorio/buscar-pastas](https://manual.arquivar.com/guia-do-cliente/arqsign/administracao-integracoes/api/metodos-disponiveis-na-api/2.diretorios/2.1.post-api-v1-diretorio-buscar-pastas)
{% endhint %}
