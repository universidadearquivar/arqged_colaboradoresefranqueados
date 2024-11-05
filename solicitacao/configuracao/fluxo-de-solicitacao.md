# 🔹 Fluxo de Solicitação

Nesta tela são exibidos todos os fluxos da unidade ou cliente selecionado no campo “Empresa”.&#x20;

<figure><img src="../../.gitbook/assets/solicita01.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Aqui são criados os fluxos das solicitações possíveis, ou seja, são configuradas as fases para que os serviços de consulta e devolução necessitam para que sejam executados dentro do sistema. &#x20;

<figure><img src="../../.gitbook/assets/solicita02.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Ícone Adicionar:** Utilizado para cadastrar um novo fluxo.  &#x20;

**Ícone Editar:** Utilizado para editar as informações do fluxo selecionado.&#x20;

**Ícone Visualizar:** Utilizado para apresentar as informações do fluxo. &#x20;

**Ícone Excluir:** Utilizado para excluir o fluxo selecionado.&#x20;

## Dados Gerais

Ao clicar em adicionar é habilitada a tela **Dados Gerais do processo de Solicitação** para preenchimento dos dados iniciais:

<figure><img src="../../.gitbook/assets/image (84).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**"Nome da Unidade/Cliente" e "Tipo de Fluxo":** Estes campos dão preenchidos de forma automática, conforme informação selecionada no campo anterior**,** se selecionada a Unidade, automaticamente o Tipo de Fluxo será preenchido como “Guarda Terceirizada” se selecionado o cliente, automaticamente o Tipo de Fluxo será preenchido como “Guarda Interna”.

**Número Máximo de itens:** Informe o limite de itens que deve ser permitido em cada pedido.&#x20;

* **Exemplo:** Se for definido limite de 100 itens por pedido e reservados 300 itens, serão criados 3 pedidos com 100 itens cada. Geralmente é utilizado o limite de 100 itens por pedido.

**Status:** Informe se processo ativo ou inativo.&#x20;

**Nome do Processo de Solicitação:** Informe o nome do processo, por exemplo "Solicitação de Consulta" ou "Solicitação de Devolução".

**Tipo de Processo:** Selecione se o fluxo criado atende ao processo de “Solicitação de Consulta” ou “Solicitação de Devolução”. &#x20;

Ao clicar em salvar, se o processo estiver sendo criado para a Unidade Arquivar, é habilitada a opção de seleção dos clientes que deverão seguir com o fluxo criado.&#x20;

Selecione o cliente e clique em adicionar.&#x20;

<figure><img src="../../.gitbook/assets/image (85).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Repita o processo até que sejam inseridos todos os clientes desejados.&#x20;

Para excluir um cliente da lista, selecione e clique no ícone excluir.&#x20;

<figure><img src="../../.gitbook/assets/image (86).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="danger" %}
<mark style="color:red;">Se o cliente não estiver vinculado a um processo de consulta, ele não conseguirá prosseguir com o processo de solicitação no sistema ou gerar um pedido para a requisição.</mark>&#x20;

<mark style="color:red;">Quando o processo for de Guarda Interna (CEDOC), não é apresentada a opção de seleção de “Clientes que seguirão o fluxo”, o processo fica vinculado automaticamente ao cliente informado no início do processo.</mark>
{% endhint %}

Concluído o preenchimento de todas as informações solicitadas na tela, clique "Salvar".

***

## Aba Processo

Nesta aba, é feita a definição de quais as etapas serão utilizadas no fluxo.

<figure><img src="../../.gitbook/assets/image (87).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Coluna Status:** São exibidas as etapas que podem ou não serem utilizadas. Por padrão, todas as etapas são apresentadas com seleção para utilização, é importante validar se realmente as etapas de “Aprovação” e “Confirmado” serão utilizadas, elas são de uso opcional e servem como “Validação” do processo para alguns atores. As demais etapas são de utilização obrigatória.

* **Aprovação:** Para transformar uma reserva em um pedido, é necessária uma ação de aprovação do responsável no cliente, ou seja, ele precisa acessar o Pedido e clicar em “Aprovar”, caso contrário, o pedido não segue para atendimento.
* **Triagem**: Nesta etapa o atendente seleciona os pedidos que serão tratados e imprime as guias de busca.
* **Separação:** Neste momento atendente vai até o documento físico e coleta aqueles que serão disponibilizados para consulta.
* **Fechamento:** Nesta etapa é realizada a digitalização dos documentos solicitados em formato digital e preparação para envio dos documentos solicitados no formato físico.
* **Confirmado:** Após realizado todo o processo de atendimento da devolução, o responsável pelo processo precisa acessar o sistema e “Confirmar” para que ele siga para o encerramento do pedido, isso fará com que o documento volte a ficar disponível para novas solicitações no sistema.

{% hint style="info" %}
<mark style="color:blue;">Quando o fluxo for para Guarda Interna as etapas apresentadas serão:</mark>&#x20;

* <mark style="color:blue;">Aguardando</mark>&#x20;
* <mark style="color:blue;">Recebido</mark>&#x20;
* <mark style="color:blue;">Conferido</mark>&#x20;
* <mark style="color:blue;">Guardado</mark>&#x20;

<mark style="color:blue;">Sendo neste caso de uso opcional apenas a etapa “Guardado”, as demais são de uso obrigatório.</mark>&#x20;
{% endhint %}

**Coluna Descrição:** Exibe um breve relato para cada status existente.&#x20;

**Coluna Usar Etapa:** Exibe um checkbox para selecionarmos qual etapa deve ser utilizada, as que não forem utilizadas devem ser mantidas sem seleção.&#x20;

**Coluna Usar Coletor:** É possível definir o uso do coletor nas etapas de separação e fechamento para leitura dos códigos utilizados, porém, não existe uma integração de automação do processo pelo uso do coletor no ArqGED. Geralmente esta opção não é utilizada.&#x20;

**Opções de destino após a separação:** É utilizado para identificar o que deve ser feito com o pedido recebido. Informe o texto e clique “Adicionar +”, estas opções serão apresentadas como “botões” para o atendente responsável evoluir com o atendimento conforme realização das atividades no sistema.&#x20;
