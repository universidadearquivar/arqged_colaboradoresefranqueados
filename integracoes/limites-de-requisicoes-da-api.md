# 🟩 Limites de Requisições da API

## Limite Rate

O limite rate é uma medida para proteger a aplicação de ataques ou mal uso do recurso de API.

O limite rate é determinado com base no número de solicitações que o seu aplicativo envia ao software em uma janela de tempo. Este limite é por Cliente no ArqGED, e a janela de tempo controlada são as listadas abaixo:

· Dentro do intervalo de 1 segundo a API do ArqGED poderá receber 4 requisições.

· Dentro do intervalo de 1 minuto a API do ArqGED poderá receber 240 requisições.

· Dentro do intervalo de 1 hora a API do ArqGED poderá receber 2.400 requisições.

| Tempo                                      |          Número de Requisições          |
| ------------------------------------------ | :-------------------------------------: |
| <mark style="color:purple;">Segundo</mark> |   <mark style="color:purple;">4</mark>  |
| <mark style="color:red;">Minuto</mark>     |   <mark style="color:red;">240</mark>   |
| <mark style="color:green;">Hora</mark>     | <mark style="color:green;">2.400</mark> |

{% hint style="danger" %}
<mark style="color:red;">Se o seu aplicativo ultrapassar este limite, a API do ArqGED não irá retornar resultado.</mark>
{% endhint %}
