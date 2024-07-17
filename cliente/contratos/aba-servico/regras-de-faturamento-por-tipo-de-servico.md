# ➡️ Regras de faturamento por tipo de serviço

## Serviços de software

### ArqGED

Habilita a utilização do software ArqGED para o cliente.&#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento**: Periódico&#x20;
* **Quantidade a ser faturada:** Para este tipo de serviço, a quantidade a ser faturada sempre será a definida no campo “Preço do Pacote Periódico”, que neste caso é preenchido automaticamente com o valor 1. Não há cobrança de pacote unitário para esse serviço.

### ArqAPI

Habilita a cobrança de requisições excedentes realizadas ao ArqGED por meio da API de integração.

* **Forma de Controle:** Automático
* **Tipo de Faturamento:**
* **Quantidade a ser faturada:** Para este tipo de serviço, a quantidade a ser faturada sempre será a definida considerando as informações existentes no campo “Unidade de Medida para o Limite Gratuito” e "Qtde para Limite Gratuito". [**Clique aqui e veja um exemplo de cálculo.** ](https://arquivar.gitbook.io/manual-arqged-or-colaboradores-e-franqueados/cliente/contratos/aba-servico/exemplos-de-calculo#arqapi)

### ArqSEARCH&#x20;

Habilita a busca por arquivos e metadados dentro do sistema. &#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Para este tipo de serviço, a quantidade a ser faturada sempre será a definida no campo “Preço do Pacote Periódico”, que neste caso é preenchido automaticamente com o valor 1. Não há cobrança de pacote unitário para esse serviço.

### ArqNFe&#x20;

Habilita o serviço de captura das notas fiscais emitidas pelo cliente, salvando automaticamente os arquivos PDF e XML da nota dentro do ArqGED. &#x20;

* **Forma de Controle:** Manual&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Para este tipo de serviço, a quantidade a ser faturada sempre será a definida no campo “Preço do Pacote Periódico”. A cobrança desse serviço deve ser feita por CNPJ para o qual o cliente deseja emitir notas fiscais. No campo “Pacote Periódico” deve ser informada a quantidade de CNPJs que irão compor o pacote periódico e no campo “Preço do Pacote Periódico” deve ser informado o preço do pacote total que será cobrado, considerando todos os CNPJs. [Clique aqui e veja um exemplo de cálculo. ](exemplos-de-calculo.md#arqnfe)

### ArqINDEX&#x20;

Habilita o serviço de captura de imagens por meio da digitalização do documento no scanner, criação do arquivo em XML, leitura do arquivo XML, criação de fila de indexação para as imagens e disponibilização das imagens digitalizadas no ArqGED para consulta do usuário.&#x20;

* **Forma de Controle:** Manual&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada**: Para este tipo de serviço, a cobrança será feita por número de páginas hospedadas dentro do ArqGED que tenham sido processadas pelo ArqINDEX no período de apuração do faturamento. Além disso, as páginas devem ser do cliente e da unidade em questão.&#x20;

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqOCR no ArqSCAN

Habilita o serviço de realização de OCR (Optical Character Recognition, ou Reconhecimento de Caractere Óptico) das páginas capturadas pelo ArqSCAN, ou seja, converte arquivos em PDF que sejam do tipo imagem para PDF com texto legível.

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Para este tipo de serviço, a cobrança será feita por número de páginas que foram processadas com OCR dentro do ArqSCAN no período de apuração do faturamento. Além disso, as páginas devem ser do cliente e da unidade em questão. [Clique aqui e veja um exemplo de cálculo.](exemplos-de-calculo.md#arqscan-+-arqocr)

{% hint style="danger" %}
<mark style="color:red;">**A cobrança do ArqOCR e ArqSCAN deve ser feita separadamente caso o cliente tenha os dois serviços contratados.**</mark>
{% endhint %}

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqSCAN&#x20;

Serviço de digitalização de páginas.&#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Para este tipo de serviço, a cobrança será feita por número de páginas que foram digitalizadas pelo ArqSCAN no período de apuração do faturamento. Além disso, as páginas devem ser do cliente e da unidade em questão.

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqSIGN

Habilita o serviço de assinatura eletrônica de documentos que não estejam vinculados a nenhum fluxo dentro do sistema.

*   **Forma de Controle:** Automático&#x20;

    **Tipo de Faturamento:** Periódico&#x20;

    **Quantidade a ser faturada:** Para este tipo de serviço, a cobrança será feita por número de arquivos assinados no período de apuração do faturamento. Além disso, as páginas devem ser do cliente e da unidade em questão. A cobrança não deve ser feita por assinatura nem por número de páginas assinadas, e sim por arquivo assinado.&#x20;

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqSIGN no ArqFLOW

Habilita o serviço de assinatura eletrônica de documentos. A diferença deste serviço para o serviço “ArqSIGN” é que neste caso, são contabilizadas as assinaturas realizadas em documentos dentro de algum fluxo do ArqFLOW.

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Para este tipo de serviço, a cobrança será feita por número de arquivos assinados no período de apuração do faturamento. Além disso, as páginas devem ser do cliente e da unidade em questão. A cobrança não deve ser feita por assinatura nem por número de páginas assinadas, e sim por arquivo assinado. &#x20;

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqSTORAGE (Total)

Serviço de armazenamento de arquivos dentro do ArqGED, incluindo os arquivos deletados que permanecem salvos no sistema por backup.

*   **Forma de Controle:** Automático&#x20;

    **Tipo de Faturamento:** Periódico&#x20;

    **Quantidade a ser faturada:** Para este tipo de serviço, a cobrança será feita por espaço de armazenamento de arquivos ativos e inativos armazenados no ArqGED. Também são contabilizados os arquivos gerados por download em massa. O tamanho de todos os arquivos armazenados é somado e convertido em gigabytes, e a cobrança é feita pela quantidade de GB consumidos.&#x20;

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqSTORAGE (Ativo)

Serviço de armazenamento de arquivos dentro do ArqGED. A diferença deste serviço para o “ArqSTORAGE (Total)” é que neste caso só são considerados arquivos ativos, ou seja, que não foram deletados.

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Para este tipo de serviço, a cobrança será feita por espaço de armazenamento de arquivos ativos armazenados no ArqGED. Também são contabilizados os arquivos gerados por download em massa. O tamanho dos arquivos armazenados é somado e convertido em gigabytes, e a cobrança é feita pela quantidade de GB consumidos.&#x20;

{% hint style="danger" %}
<mark style="color:red;">**O ideal é que a cobrança seja sempre feita como ArqSTORAGE (Total), já que de qualquer forma o sistema realiza o backup e mantém os arquivos dos clientes armazenados mesmo após a exclusão. Sendo assim, mesmo que o cliente pague apenas pelo serviço Ativo, consumirá a mesma quantidade de espaço de armazenamento do serviço Total.**</mark>
{% endhint %}

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqTRAFFIC

Cobrança do serviço de tráfego de imagens, ou seja, cobrança por quantidade de downloads de imagens realizados.

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Para este tipo de serviço, a cobrança será feita pelo tamanho dos arquivos baixados. O tamanho dos arquivos baixados é somado e convertido em megabytes, e a cobrança é feita pela quantidade de tráfego de MB no período.

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqUSERS

Cobrança dos usuários ativos e inativos do cliente cadastrados no sistema no período de faturamento.

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Para este tipo de serviço, a cobrança será feita por quantidade de usuários do cliente com status ativo ou bloqueado no período do faturamento. Também serão somados usuários com status inativo, desde que a inativação tenha ocorrido em data anterior ou durante o período do faturamento. [Clique aqui e veja um exemplo de cálculo.](exemplos-de-calculo.md#arqusers)

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqDOC

Serviço de caixas do cliente arquivadas fisicamente e registradas no sistema ArqGED.

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento**: Periódico&#x20;
* **Quantidade a ser faturada**: Neste serviço a cobrança será feita por quantidade de caixas do tipo pai (container) arquivadas, que tenham sido criadas antes ou durante o período do faturamento. Caixas excluídas durante o período de faturamento também devem ser cobradas. [Clique aqui e veja exemplos de cálculos.](exemplos-de-calculo.md#pacote-periodico-+-pacote-unitario)

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqFLOW&#x20;

Habilita a ativação de fluxos de processos no ArqGED.&#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Neste serviço a cobrança será por número de fluxos ativados durante o período de faturamento que sejam do cliente e unidade em questão e do serviço em questão.  Em um mesmo contrato é possível associar o serviço ArqFLOW mais de uma vez, por isso é importante que no campo “Nome Espelho” seja informado o tipo de fluxo ao qual o serviço que está sendo cadastrado se refere. [Clique aqui para ver um exemplo.](exemplos-de-calculo.md#arqflow)

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqAUDIT por Regra

Habilita a criação de regras de auditoria em processos no ArqGED. Neste tipo de serviço é possível cobrar tanto por regras vinculadas a uma lista quanto por regras sem vínculo. &#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Neste serviço a cobrança será por número de regras criadas durante o período de faturamento que sejam do cliente, unidade e do serviço em questão, e que não tenham sido deletadas. m um mesmo contrato é possível associar o serviço ArqAUDIT por Regra mais de uma vez, por isso é importante que no campo “Nome Espelho” seja informado o tipo de regra à qual o serviço que está sendo cadastrado se refere.

{% hint style="warning" %}
<mark style="color:orange;">**Neste serviço, o ideal é que seja cadastrada pelo menos a cobrança de pacote unitário, mesmo que não haja cobrança de mensalidade periódica.**</mark>
{% endhint %}

### ArqAUDIT por Lista

Habilita a criação de regras de auditoria em processos no ArqGED que estejam vinculadas a listas previamente cadastradas no menu Lista do ArqGED.

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Neste serviço a cobrança será por número de regras criadas durante o período de faturamento que sejam do cliente, unidade e do serviço em questão, e que não tenham sido deletadas. As regras devem estar vinculadas a uma lista e a cobrança deve ser feita por lista. Clique aqui para conferir um exemplo. Em um mesmo contrato é possível associar o serviço ArqAUDIT por Lista mais de uma vez, por isso é importante que no campo “Nome Espelho” seja informado o tipo de regra à qual o serviço que está sendo cadastrado se refere. Também é possível dentro de uma mesma lista efetuar cobranças distintas para itens ativos ou inativos.

***

## Gestão de documentos

### Serviços de Guarda

Serviços relacionados ao aluguel de espaço físico para abrigar as caixas do cliente.

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:**&#x20;
  * Nestes serviços a cobrança será feita por quantidade de caixas arquivadas do tipo container (pai). Uma caixa pai abriga três subcaixas (filhas), portanto essas subcaixas não são cobradas, já que estão ocupando o mesmo espaço da caixa pai.&#x20;
  * As caixas devem ter sido criadas antes ou durante o período de faturamento. Não são consideradas caixas canceladas, ou seja, caixas que foram criadas, mas não receberam documentos do cliente e não estão sendo utilizadas.&#x20;
  * Caixas excluídas, ou seja, que foram ou serão descartadas pelo cliente, devem ser cobradas caso a data da exclusão seja maior ou igual ao período de faturamento.
  * [Clique aqui e veja um exemplo de cálculo.  ](exemplos-de-calculo.md#servicos-de-guarda)&#x20;

{% hint style="warning" %}
<mark style="color:orange;">**Nos serviços “Guarda de Container Gerenciada” e “Guarda de Container Simples” a cobrança deve ser feita considerando a quantidade de caixas associadas ao serviço que está sendo faturado e foi indicado na criação da caixa, no menu Caixa ou Pasta > Criar > Caixa da Unidade. Só podem ser cobradas caixas que tenham o serviço cadastrado anteriormente no contrato do cliente.**</mark>
{% endhint %}

### Consulta de Caixa

Serviço disponível para clientes que já possuem o serviço de guarda contratado e solicitam poder consultar o conteúdo do arquivo. O cliente informa quais caixas deseja consultar via menu Solicitação > Consulta e é feita a reserva dessas caixas.

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:**&#x20;
  * Neste serviço a cobrança será feita por número de caixas solicitadas, considerando a prioridade e o tipo de caixa. &#x20;
  * É possível cobrar preços e definir prioridades diferentes para cada tipo de caixa. Para efetuar a cobrança, o sistema vai verificar se a solicitação do cliente está inclusa nos serviços contratados. &#x20;
  * A prioridade e o tipo de uma caixa devem ser cadastrados ao se realizar a criação dessa caixa no sistema, no menu Caixa ou Pasta > Criar > Caixa da Unidade.&#x20;
  *   A busca deve ser feita em caixas do cliente e unidade em questão.&#x20;

      Não são consideradas subcaixas. Serão cobradas apenas caixas do tipo pai.&#x20;
  * São contabilizadas as consultas fechadas durante o período de faturamento, ou seja, consultas que foram atendidas até o último dia do período. &#x20;
  * Não podem ser solicitadas nesse serviço consultas TEMP, ou seja, consulta a caixas que estão guardadas com a Unidade, mas ainda não foram preparadas para disponibilização para o cliente.&#x20;

{% hint style="warning" %}
<mark style="color:orange;">**A prioridade de uma caixa é o SLA de atendimento de consulta, ou seja, o tempo médio que a Unidade possui para atender a uma solicitação de consulta do cliente, que pode ser Normal, Prioritário, Urgente ou Extra. A Unidade deverá definir qual o tempo médio de cada SLA de atendimento. O SLA deve considerar também o volume que pode ser atendido em cada solicitação.**</mark>
{% endhint %}

### Consulta de Documento

Serviço disponível para clientes que já possuem o serviço de guarda contratado e solicitam poder consultar documentos específicos dentro das caixas. O cliente informa qual documento deseja consultar via menu Solicitações > Consulta e é feita a entrega desses documentos. Neste serviço deve ser cobrada também a consulta TEMP, que é a consulta às caixas que estão sob a guarda da Unidade, mas ainda não foram preparadas, organizadas, indexadas etc.

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:**&#x20;
  * Neste tipo de serviço a cobrança é feita por quantidade de buscas realizadas, ou seja, quantas vezes o atendente teve que procurar dentro de uma caixa o documento solicitado pelo cliente. &#x20;
  * O valor cobrado deve considerar a prioridade e o tipo de caixa na qual o documento está arquivado. É possível cobrar preços e definir prioridades diferentes para cada tipo de caixa.
  * Para efetuar a cobrança, o sistema vai verificar se a solicitação do cliente está inclusa nos serviços contratados. A prioridade e o tipo de uma caixa devem ser cadastrados ao se realizar a criação dessa caixa no sistema, no menu Caixa ou Pasta > Criar > Caixa da Unidade.&#x20;
  * A busca deve ser feita em caixas do cliente e unidade em questão.&#x20;

### Consulta de Subcaixa&#x20;

Serviço disponível para clientes que já possuem o serviço de guarda contratado e solicitam poder consultar uma subcaixa (filha) que esteja inserida em uma caixa do tipo container (pai). O cliente informa quais subcaixas deseja consultar via menu Solicitação > Consulta e é feita a reserva dessas subcaixas.&#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:**&#x20;
  * Neste serviço a cobrança será feita por número de subcaixas solicitadas, considerando a prioridade e o tipo de caixa. &#x20;
  * É possível cobrar preços e definir prioridades diferentes para cada tipo de caixa. Para efetuar a cobrança, o sistema vai verificar se a solicitação do cliente está inclusa nos serviços contratados. &#x20;
  * A prioridade e o tipo de uma caixa devem ser cadastrados ao se realizar a criação dessa caixa no sistema, no menu Caixa ou Pasta > Criar > Caixa da Unidade.&#x20;
  * A busca deve ser feita em caixas do cliente e unidade em questão.&#x20;
  * São contabilizadas as consultas fechadas durante o período de faturamento, ou seja, consultas que foram atendidas até o último dia do período. &#x20;
  * Não podem ser solicitadas nesse serviço consultas TEMP, ou seja, consulta a caixas que estão guardadas com a Unidade, mas ainda não foram preparadas para disponibilização para o cliente

### Criação de Caixa&#x20;

Cobrança das caixas de papelão vendidas ao cliente para armazenamento de documentos.&#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:**&#x20;
  * Deve ser cobrado o valor de custo de cada caixa utilizada pelo cliente, observando o tipo de caixa.&#x20;
  * Deve ser estipulado um preço específico para cada tipo de caixa.&#x20;
  * Serão cobradas as caixas que sejam do cliente e unidade em questão, que sejam do tipo container (pai) e com data de criação dentro do período de apuração do faturamento.&#x20;
  * Não devem ser cobradas caixas com o status de cancelada, ou sejam, que foram criadas, mas não foram utilizadas pelo cliente.

### Devolução de Caixa&#x20;

Serviço de devolução das caixas retiradas para consulta.&#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Deve ser cobrado o valor por caixa devolvida dentro do período de apuração do faturamento, que seja do cliente e unidade em questão.&#x20;

### Devolução de Documentos&#x20;

Serviço de devolução dos documentos retirados para consulta.&#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Deve ser cobrado o valor por documento devolvido dentro do período de apuração do faturamento, que seja do cliente e unidade em questão.&#x20;

### Disponibilização de Documento via E-mail&#x20;

Serviços de disponibilização via e-mail para o cliente dos documentos digitalizados e hospedados no ArqGED.&#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Neste serviço serão somadas as consultas de caixa, de documentos, de subcaixas e consultas TEMP realizadas e atendidas durante o período de faturamento. A cobrança será por número de cópias digitalizadas e enviadas para o cliente.

### Fotocópia&#x20;

Serviços de disponibilização de fotocópia enviada para o cliente dos documentos digitalizados e hospedados no ArqGED.&#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Neste serviço serão somadas as consultas de caixa, de documentos, de subcaixas e consultas TEMP realizadas e atendidas durante o período de faturamento. A cobrança será por número de cópias feitas e enviadas para o cliente.&#x20;

### Indexação Automática&#x20;

Serviço de cadastro do documento no sistema ArqGED via menu Documento > Cadastrar. &#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:** Este serviço será cobrado por quantidade de registros inseridos no sistema ArqGED dentro do período de faturamento, que sejam do cliente e unidade em questão.  Para ser cobrada a indexação não poderá ter sido feita por um usuário do cliente, porque neste caso, ele próprio executou o serviço então o serviço não deverá ser cobrado.&#x20;

### Sala de Consulta&#x20;

Quando o volume de documentos do cliente é muito grande ou o arquivo do cliente está desorganizado, ao solicitar uma consulta o cliente pode requerer o serviço de Sala de Consulta, que é a disponibilização de um espaço dentro da unidade para que o cliente possa comparecer no dia e horário agendados e ele próprio localizar e consultar os documentos que deseja. &#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:**&#x20;
  *   Neste serviço será cobrado o aluguel do espaço pelo período em que o cliente o utilizou. &#x20;

      Essa cobrança deve ser feita por período de quatro horas (manhã ou tarde). Caso o cliente solicite o dia inteiro, serão cobradas duas unidades do serviço.&#x20;
  * [Clique aqui para conferir um exemplo. ](exemplos-de-calculo.md#sala-de-consulta)
  * Não se cobra mais que duas reservas de salas por dia.&#x20;
  * Ao solicitar uma consulta de caixa ou documento via menu Solicitação > Consulta, o cliente deve informar que a consulta será feita in loco e informar o dia e turno (manhã, tarde ou dia inteiro) em que ele irá comparecer à Unidade para realizar a pesquisa.&#x20;
  * A quantidade de caixas ou documentos solicitados para consulta não interfere no valor cobrado, já que o cliente estará pagando apenas pelo uso do espaço. &#x20;
  * Será cobrado valor excedente apenas se o cliente extrapolar o período solicitado.&#x20;
  * Se houver somente um período reservado para o mesmo dia, mesmo se forem várias solicitações, se cobra somente 1 unidade.

### Substituição de Caixa&#x20;

Serviço de troca da caixa de papelão dos arquivos sob a guarda da Arquivar. As caixas de armazenamento têm uma durabilidade média de cinco anos. Após esse período é necessário realizar a troca para evitar possíveis avarias aos documentos arquivados.&#x20;

* **Forma de Controle:** Automático&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:**&#x20;
  * Deve ser cobrado o valor de custo de cada caixa que será substituída, observando o tipo de caixa e se a nova caixa é nova ou usada.&#x20;
  * Deve ser estipulado um preço específico para cada tipo de caixa.&#x20;
  * Serão cobradas as caixas que sejam do cliente e unidade em questão, que sejam do tipo container (pai) e com data de criação dentro do período de apuração do faturamento.&#x20;
  * Não devem ser cobradas caixas com o status de deletada, ou sejam, que foram criadas, mas foram deletadas pelo cliente.&#x20;

### Transporte&#x20;

Serviço de translado das caixas e documentos solicitados para consulta pelo cliente, da Unidade para o cliente e do cliente para a Unidade.

* **Forma de Controle:** Manual&#x20;
* **Tipo de Faturamento:** Periódico&#x20;
* **Quantidade a ser faturada:**&#x20;
  * Esse tipo de serviço tem controle manual e deve-se informar no campo “Pacote Unitário” a quantidade de caixas que será transportada e no campo “Preço do Pacote Unitário” o valor que será cobrado para se transportar aquela quantidade de caixas, observando o limite de volume que pode ser transportado pelo veículo que for atender o pedido. &#x20;
  * Também é possível realizar a cobrança informando no campo “Nome Espelho” a quantidade limite de caixas que podem ser transportadas, inserindo-se no campo “Pacote Unitário” o valor 1 e no campo “Preço do Pacote Unitário” o valor que será cobrado por transporte daquele volume.&#x20;
  * [Clique aqui para conferir um exemplo.](exemplos-de-calculo.md#transporte)&#x20;

### N.A &#x20;

Serviços variados que podem ser oferecidos pela Unidade ao cliente, que não estejam entre os serviços disponíveis para cadastro no ArqGED, como digitalização, organização, consultoria, auditoria, treinamento, ente outros.

* **Forma de Controle:** Os serviços N.A pode ter controle Manual ou Automático&#x20;
* **Tipo de Faturamento:** Periódico ou Parcelado&#x20;
*   **Quantidade a ser faturada:** Esses serviços têm lançamento manual, porque não é possível para o sistema identificar como deverá faturar a quantidade contratada. &#x20;

    &#x20;
