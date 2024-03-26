# 🔹 Parâmetros Gerais

No menu Parâmetros Gerais são configurados os locais de trabalho que serão posteriormente associados à aplicação ArqIndex. Cada Unidade ou cliente pode ter um ou mais locais de trabalho configurados, mas a aplicação ArquIndex pode ter relacionado apenas um local de trabalho.

{% hint style="info" %}
<mark style="color:blue;">**Local de trabalho**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">é o termo utilizado para configuração criada com os parâmetros de execução da aplicação ArqIndex. Por exemplo, a Unidade Arquivar Qualidade possui um local de trabalho chamado "Documentos de Funcionários".</mark>
{% endhint %}

O nome do local de trabalho pode ser aquele que o usuário desejar. Posteriormente esse local criado será relacionado a um fluxo de trabalho e associado à aplicação ArquIndex.&#x20;

## Parâmetros Gerais – Tela inicial&#x20;

**Campo Empresa:** Utilizado para selecionar o cliente ou a unidade Arquivar relacionada ao cliente.&#x20;

**Ícone Adicionar:** Utilizado para configurar um novo local de trabalho.&#x20;

**Ícone Editar:** Utilizado para editar um local de trabalho já existente.&#x20;

**Ícone Visualizar:** Utilizado para visualizar os detalhes da configuração do local de trabalho selecionado.   &#x20;

**Ícone Excluir:** Utilizado para excluir o local de trabalho selecionado.&#x20;

**Coluna Empresa:** Exibe o cliente ou unidade Arquivar selecionado.&#x20;

**Coluna Local de Trabalho:** Exibe o nome dado ao local de trabalho.    &#x20;

<figure><img src="../../.gitbook/assets/conf01.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Configuração do local de trabalho&#x20;

Para iniciar a configuração de um local de trabalho, selecione a "Empresa" e clique no ícone "Adicionar".

<figure><img src="../../.gitbook/assets/conf27.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

### Aba Dados Gerais&#x20;

Na tela “Adicionar Registro”, informe um nome para o local de trabalho que está sendo configurado.  &#x20;

<figure><img src="../../.gitbook/assets/conf02.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Ao longo do processo de indexação um arquivo de documento fica hospedado em diferentes locais do servidor, chamados de “Diretório para Armazenamento”.

**Local dos arquivos de Entrada:** Quando um documento é digitalizado ele gera dois arquivos: um XML e um PDF (imagem), que ficam hospedados nesse local. Quando o robô do ArqIndex inicia o processo de leitura dos arquivos XML e verifica se todas as informações estão corretas.&#x20;

**Local dos arquivos em Processo:** Local para onde os arquivos são enviados após a leitura inicial do XML pelo robô. Os arquivos dessa pasta ficam em uma fila de trabalho aguardando que sejam indexados. &#x20;

**Local dos arquivos em Exportação:** Local em que os arquivos ficam hospedados quando já foram indexados e estão prontos para serem exportados para o ArqGED. Quando a exportação é executada, os documentos são gravados na base de dados do sistema e podem ser consultados por meio da [Localização Simples](../../documento/localizacao-simples.md), [Localização Avançada](../../documento/localizacao-avancada.md) ou tela [Explorar](../../documento/explorar/). &#x20;

**Host/IP:** Endereço da máquina onde o robô do ArqIndex está instalado.&#x20;

Esses campos ficam desabilitados nessa tela porque a sua configuração deve ser feita quando o aplicativo (robô) for instalado. As configurações feitas durante a [instalação do aplicativo ArqIndex](aplicativo-arqindex.md#instalacao-do-aplicativo-arqindex) são espelhadas nessa tela.  &#x20;

<figure><img src="../../.gitbook/assets/conf03.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Em “Programação do processamento do Robô” é definida a periodicidade da leitura dos arquivos XML, da indexação automática, da conversão e da exportação dos arquivos do cliente, que são as rotinas do processo de indexação de um documento executadas pelo próprio sistema.  &#x20;

Esses campos definem a periodicidade em que cada um dos processos deve ocorrer, que pode ser durante 24 horas ou durante um horário pré-definido. Os campos “Intervalo” devem ser preenchidos com os minutos de intervalo de execução de cada processo, que por padrão é de 5 minutos.  &#x20;

{% hint style="info" %}
<mark style="color:blue;">**EXEMPLO:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">É possível que o usuário queira definir que os processos do robô sejam executados em um horário em que não há concorrência no uso da máquina. Neste caso, pode ser definido, por exemplo, o horário pré-definido 17:00 às 08:00.</mark>   &#x20;
{% endhint %}

<figure><img src="../../.gitbook/assets/conf04.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

### Aba Log

Depois de configurado um local de trabalho, clicando no ícone “Visualizar” é exibida a aba Log, em que são apresentados os logs do robô de processamento, ou seja, as informações de todas as movimentações dos processos que foram realizados nos arquivos escaneados e indexados.  &#x20;

No campo “Processo” selecione a etapa do fluxo de trabalho da qual deseja visualizar os logs executados.&#x20;

<figure><img src="../../.gitbook/assets/conf05.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Coluna Tipo:** Nesta coluna é apresentado o ícone que representa o tipo de log, que pode ser de informação ou de erro.&#x20;

**Coluna Data/Hora:** Apresenta as informações de data e hora de quando a ação apresentada foi executada pelo robô do ArqIndex.&#x20;

**Coluna Cliente:** Apresenta o nome do cliente selecionado.&#x20;

**Coluna Lote/Id Lote:** Apresenta o Id do lote, quando selecionada a etapa de “Leitura do XML” no campo “Processo”. &#x20;

**Coluna Descrição:** Apresenta informações do log ou os erros encontrados no processamento do arquivo, se houverem.&#x20;

<figure><img src="../../.gitbook/assets/conf06.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>
