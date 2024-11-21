# 🔹 Consulta

Nesta tela são exibidas as solicitações do cliente feitas pelo menu Solicitações > Consulta. Toda a reserva transformada em **Pedido**, fica disponível para atendimento neste local, seja para atendimento realizado pela Unidade Arquivar (Guarda Terceirizada) ou pelo CEDOC do cliente (Guarda Interna).

<figure><img src="../../.gitbook/assets/image (101).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">O painel de atendimento é único e exibe todos os tipos de pedidos realizados no ArqGED:</mark>

* <mark style="color:blue;">Documento original</mark>
* <mark style="color:blue;">Documento digitalizado</mark>
* <mark style="color:blue;">Documento cópia</mark>
* <mark style="color:blue;">Caixa</mark>
* <mark style="color:blue;">Subcaixa</mark>
{% endhint %}

Os campos exibidos no cabeçalho da página são campos disponíveis para “pesquisa” de pedidos.

<figure><img src="../../.gitbook/assets/image (102).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Prioridade:** Exibe para seleção as opções de atendimento disponíveis, geralmente são utilizadas as opções de consulta "normal e urgente".

**Caixa ou Subcaixa:** Campo disponível para inserir o número da caixa ou subcaixa que deseja consultar o pedido.

**Código Documento:** Campo disponível para consultar os pedidos por código do registro.

**Código Consulta:** Permite a localização do pedido pelo número gerado no atendimento da solicitação.

**Tipo de Guarda:** Exibe as opções de guarda sendo elas guarda terceirizada ou guarda interna. Por padrão este campo já aparece preenchido conforme o tipo de usuário logado.

**Empresa:** Quando o usuário logado for de Unidade, será apresentada a lista de clientes de guarda terceirizada.

**Data Início / Data Fim:** Permite a busca de todas as solicitações abertas em determinado período.

**Pesquisar:** Ao clicar neste botão, é realizada a busca dos pedidos conforme dados informados para busca.

<figure><img src="../../.gitbook/assets/image (103).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Editar:** Permite a edição do pedido, selecione o pedido e clique em editar.

**Visualizar:** Permite a visualização do pedido, selecione o pedido e clique em visualizar.

**Distribuir:** O ícone é habilitado na tela de atendimento a consulta sempre que +1 pedido com status “Em Triagem” estiver selecionado no GRID.

Ao pressionar este ícone a aplicação abre uma modal com os campos “Atendente Responsável” e “Destino”.

<figure><img src="../../.gitbook/assets/image (104).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Desta forma o Gerente do atendimento pode realizar a definição do atendente responsável e do destino das solicitações selecionadas em lote.

Não é obrigatório informar os dois campos, ele pode informar somente um campo, desta forma, se for selecionado novamente um universo, e neste pelo menos 1 pedido já tiver a informação de “Atendente Responsável”, estará habilitado somente o campo “Destino” e vice e versa.

<figure><img src="../../.gitbook/assets/image (105).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Exportar:** Permite gerar um arquivo .CSV considerando:

* Informações do Pedido
* Informações dos Itens
* Informações dos Atendimento

O relatório de “Informações dos Atendimentos” é muito utilizado para validação do faturamento, pois, nele são consideradas as informações utilizadas durante o processo.

<figure><img src="../../.gitbook/assets/image (106).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Coluna Tipo:** Exibe o ícone que corresponde ao tipo de volume solicitado.

<figure><img src="../../.gitbook/assets/image (107).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">**Caixa Temporária:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Somente a unidade consegue fazer este tipo de pedido. Ele deve ser usado quando a caixa ainda não foi indexada e o setor de atendimento precisa procurar um documento dentro desta caixa para enviar ao Cliente. Desta forma nesta consulta se seleciona a caixa, é realizada a busca pelo documento que é enviado  para o cliente. Feito desta forma é gerada uma cobrança de consulta de documento e a caixa não muda o status para "Enviado ao Cliente".</mark>
{% endhint %}

**Coluna Pedido:** Exibe o número de pedido gerado no momento do envio da solicitação de consulta.

**Coluna Cliente:** Exibe o nome do cliente de cada um dos pedidos.

**Coluna Solicitante:** Exibe o nome do usuário que realizou a solicitação no sistema.

**Coluna Atendente:** Exibe o nome do colaborador responsável pelo atendimento da solicitação.

**Coluna Data Envio:** Exibe a data/hora em que o pedido foi efetivado no sistema pelo solicitante.

**Coluna Ordem:** Por padrão o campo “Ordem” sempre vem com o número “10”, e o usuário terá a possibilidade de mudar a ordem do pedido, diminuindo este número e então este pedido ficará na frente dos demais independente do seu SLA. Seria uma forma do Gerente poder priorizar um pedido por questões críticas.

Por padrão, os pedidos são ordenados com a seguinte regra:

1. Ordenados pelo campo “Ordem”
2. Ordenados pelo “Status”
3. Ordenados pelo “SLA” (o mais antigo primeiro)

**Coluna Data SLA:** Exibe a data/hora ou período limite para conclusão do atendimento da solicitação.

**Coluna Data Previsão:** Exibe a data prevista para fechamento do atendimento no sistema.

**Coluna Data Fechado:** Exibe a data de fechamento (conclusão do atendimento) do pedido no sistema.

**Coluna Status:** Exibe em qual fase do fluxo de consulta o pedido está no momento.

**Coluna Destino:** Exibe o destino do item solicitado após busca no local de acondicionamento.

Além dos filtros disponíveis no cabeçalho da tela, existe a possibilidade de aplicação de filtro nas colunas.

<figure><img src="../../.gitbook/assets/image (108).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Ao utilizar o filtro das colunas do Painel de Atendimento, fique atento aos comandos disponíveis para busca:

<figure><img src="../../.gitbook/assets/image (109).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

O ideal, quando o usuário não tiver certeza de como foi escrito o texto que busca, é informar que o filtro deverá considerar tudo que “**Contém**” o texto e informar no filtro parte da informação que deseja buscar.

<figure><img src="../../.gitbook/assets/image (110).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">O usuário</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**solicitante**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">poderá acessar o painel de atendimento para</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**visualizar**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">o andamento da sua solicitação, consultar seu pedido ou exportar dados do pedido em .CSV, porém, não é permitido ao solicitante nenhuma interação com o atendimento da demanda. Apenas o atendente da Unidade Arquivar ou do CEDOC do cliente, poderá prosseguir com o atendimento do pedido no sistema. Para o usuário solicitante não é habilitada a opção de "Editar" o pedido.</mark>
{% endhint %}

***

## Atendimento de um Pedido de Documento <a href="#atendimento-de-um-pedido-de-documento" id="atendimento-de-um-pedido-de-documento"></a>

No Painel de Atendimento, selecione o pedido que será trabalhado e clique em editar.

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F1023047207-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FtM1xGMYoU6wC7tnUUXEo%252Fuploads%252FMlckoWR6ig8PZOpiJDMw%252Fimage.png%3Falt%3Dmedia%26token%3D345bfbf0-6ffd-40db-851d-ad6fa46e8df4&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=bd8c24e0&#x26;sv=1" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

A tela de atendimento é dividida em duas abas:

### Aba Dados Gerais

