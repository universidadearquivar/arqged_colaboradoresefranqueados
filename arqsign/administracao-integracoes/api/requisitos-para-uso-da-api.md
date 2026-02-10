# ▫️ Requisitos para uso da API

1. [Acesse sua conta](https://manual.arquivar.com/guia-do-cliente/arqsign/visao-geral-da-plataforma-2.23.0#pagina-de-login-autenticacao-na-plataforma-arqsign) ou crie uma [conta teste grátis](https://manual.arquivar.com/guia-do-cliente/arqsign/visao-geral-da-plataforma-2.23.0#criacao-de-conta-teste-gratis) na Plataforma ArqSign. Depois de autenticado, clique no menu [Integrações e acesse sua API AppKey](https://manual.arquivar.com/guia-do-cliente/arqsign/administracao-integracoes/api#appkey), ID de usuário e ID de pasta.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2Fcontent.gitbook.com%2Fcontent%2FNkvKZtdmOiilgqExqFNO%2Fblobs%2Fl2GZzC238ABRg6fhvJpg%2Fintegracoes6.png&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=f13300e9&#x26;sv=2" alt=""><figcaption></figcaption></figure>

2\. Para testes, use a ferramenta Postman e para Authorization use o tipo AppKey.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2Fcontent.gitbook.com%2Fcontent%2FNkvKZtdmOiilgqExqFNO%2Fblobs%2FKMBY0wRHh4hlC3RpZAZk%2Fapi01.png&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=ed605fc6&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**Requisitos**

* Ter uma conta na plataforma ArqSign ativa.
* Ter uma [chave de acesso a API válida](https://manual.arquivar.com/guia-do-cliente/arqsign/administracao-integracoes/api#appkey). Esta chave chamamos de AppKey.
* Para o método [**POST/api/v2/processo/enviar-documento-para-assinar**](https://manual.arquivar.com/guia-do-cliente/arqsign/administracao-integracoes/api/metodos-disponiveis-na-api/1.-processo/1.1.post-api-v2-processo-enviar-documento-para-assinar), será necessário ter em mãos:

_-> ID de um usuário da conta com status ativo: para ser responsável pelos documentos que serão enviados pela API._

_-> ID de pasta: onde o documento a ser gerado deve ser armazenado na plataforma._

* Para o método [**POST/api/v2/processo/enviar-documento-para-assinar**](https://manual.arquivar.com/guia-do-cliente/arqsign/administracao-integracoes/api/metodos-disponiveis-na-api/1.-processo/1.1.post-api-v2-processo-enviar-documento-para-assinar), será necessário:

_-> Conta com status ativo e com permissão de Integração ArqSign._

_-> A conta deve possuir créditos de Envios, SMS e/ou WhatsApp, conforme necessidade. Caso a conta não possua crédito, o sistema retorna com mensagem de "saldo de créditos de Envios ou WhatsApp ou SMS insuficientes._

{% hint style="warning" %}
**A funcionalidade de** [**Diretórios**](https://manual.arquivar.com/guia-do-cliente/arqsign/processos-pastas#acesso-a-pasta-raiz-de-diretorios) **permitirá ao cliente ter várias pastas organizadoras dentro da plataforma.**
{% endhint %}
