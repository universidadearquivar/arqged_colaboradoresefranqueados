# 🟩 Localização Simples

{% @supademo/embed demoId="cmazfqpr799dpho3ruv0m8rio" url="https://app.supademo.com/demo/cmazfqpr799dpho3ruv0m8rio" %}

A Localização Simples funciona como uma busca geral, ou seja, é necessário apenas informar um termo ou código que se esteja buscando e selecionar o cliente ao qual o documento que se busca está relacionado.

<figure><img src="../.gitbook/assets/documento9.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

É possível utilizar alguns filtros para refinar a busca informando a Unidade, o Universo de Trabalho, a Árvore Organizacional e selecionando se deseja aplicar a pesquisa no universo de busca de metadados, de arquivos ou ambos.

{% hint style="warning" %}
<mark style="color:orange;">**Por padrão, o sistema realiza a busca por metadados (campos indexadores), mas se o cliente possuir os serviços ArqOCR e ArqSEARCH contratados, será possível realizar a busca pelo conteúdo dos arquivos PDF gerados via**</mark> [<mark style="color:blue;">**ArqSCAN**</mark>](explorar/modulo-arqscan.md)<mark style="color:orange;">**.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/documento10.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Ao clicar em “Pesquisar” o sistema retornará como resultado todos os registros que contenham o texto ou código informados, desde os nós da árvore do cliente até os campos de indexação dos documentos. Esse tipo de busca retorna um resultado mais amplo.

<figure><img src="../.gitbook/assets/documento11.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Ícones da tela Localização Simples

Ao concluir a busca, serão exibidos os registros encontrados. O total de registros encontrados é exibido no canto inferior direito da tela.

<figure><img src="../.gitbook/assets/doc37.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Selecionado um ou mais registros serão habilitados os ícones para as ações:

<figure><img src="../.gitbook/assets/doc36.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

### Editar

Utilizado para editar informações do registro que estiver selecionado. Será aberta a mesma tela mostrada em [Documento > Cadastrar](cadastrar.md).

### Visualizar

Utilizado para visualizar as informações do registro que estiver selecionado. Será aberta a mesma tela mostrada em [Documento > Cadastrar](cadastrar.md).

### Excluir

Utilizado para excluir o registro que estiver selecionado.

{% hint style="danger" %}
<mark style="color:red;">O ícone de exclusão só será exibido habilitado, se o usuário logado tiver a permissão ativa.</mark>
{% endhint %}

### Reservar documento

Este ícone só será habilitado se houver documento físico associado ao registro selecionado, ou seja, documentos que tenham sido castrados como de “Guarda Interna” ou “Guarda Terceirizada” na tela [Documento > Cadastrar](cadastrar.md). Neste caso será possível [solicitar a consulta](../solicitacao/consulta.md) aos documentos físicos por meio deste ícone.

### Reservar caixa

Este ícone só será habilitado se houver caixa física de documentos associada ao registro selecionado. Neste caso será possível [solicitar a consulta](../solicitacao/consulta.md) aos documentos das caixas por meio deste ícone.

### Reservar subcaixa

Este ícone só será habilitado se houver subcaixa física de documentos associada ao registro selecionado. Neste caso será possível [solicitar a consulta](../solicitacao/consulta.md) aos documentos das subcaixas por meio deste ícone.

### Exportar

Esta opção permite exportar um relatório em formato Excel com os resultados da pesquisa. É possível exportar os resultados de todos os documentos encontrados, apenas os resultados de documentos que estejam emprestados ou apenas resultados de documentos já vencidos.

<figure><img src="../.gitbook/assets/doc38.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

O relatório gerado sempre mostrará os resultados separados por nó da árvore organizacional do cliente.

<figure><img src="../.gitbook/assets/doc39.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">Relatórios com menos de 20 mil linhas, são exibidos na tela do usuário no momento da solicitação. Já os relatórios com mais de 20 mil linhas, a solicitação é encaminhada para a lista de</mark> [<mark style="color:orange;">Download em Massa</mark>](download-em-massa.md)<mark style="color:orange;">.</mark>
{% endhint %}

### Assinatura

Se o cliente possuir o serviço de Assinatura Digital contratado, será exibido o ícone “Assinatura”. Será possível realizar a assinatura em lote dos arquivos selecionados no grid de todos os arquivos dos resultados da pesquisa realizada (sendo limitado a 300 arquivos por vez).

<figure><img src="../.gitbook/assets/doc40.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Para executar a assinatura de documentos, é necessário realizar a [instalação do ArqClient](explorar/modulo-arqscan.md#instalando-atualizando-o-arqclient) na máquina onde o processo será executado.

{% hint style="warning" %}
<mark style="color:orange;">Para assinatura de documentos tratados em conformidade com o Decreto 10.278, os arquivos que atingirem 300MB ou mais deverão ser tratados com o fracionamento em partes sequenciais devidamente nomeadas. Caso haja numeração preexistente, como o número de atendimento, sugerimos utilizar essa identificação no nome do arquivo para facilitar a organização e a futura localização do registro no ArqGED.</mark>

<mark style="color:orange;">**Exemplo:**</mark>

<mark style="color:orange;">Prontuário de atendimento nº 100, o fracionamento correto do arquivo deve ser:</mark>

<mark style="color:orange;">100 parte 01/03.pdf</mark>

<mark style="color:orange;">100 parte 02/03.pdf</mark>

<mark style="color:orange;">100 parte 03/03.pdf</mark>

<mark style="color:orange;">Esse procedimento visa otimizar o manuseio e a entrega dos arquivos, evitando possíveis dificuldades no processo de assinatura do acervo.</mark>
{% endhint %}

{% hint style="danger" %}
<mark style="color:red;">Em conformidade com o Decreto nº 10.278/2020, que estabelece os requisitos técnicos para a digitalização de documentos públicos e privados, o processo de assinatura do documento digitalizado tem como finalidade atestar a integridade e a autenticidade do processo de digitalização. Dessa forma, o documento deve ser assinado digitalmente pelo responsável que realizou a digitalização.</mark>

<mark style="color:red;">No momento da assinatura digital, é gerado um</mark> <mark style="color:red;"></mark>_<mark style="color:red;">**hash**</mark>_ <mark style="color:red;"></mark><mark style="color:red;">criptográfico que garante que o arquivo não sofreu qualquer forma de alteração na digitalização. Caso o documento seja manipulado ou modificado posteriormente, esse</mark> <mark style="color:red;"></mark>_<mark style="color:red;">**hash**</mark>_ <mark style="color:red;"></mark><mark style="color:red;">é automaticamente corrompido, colocando o arquivo em desconformidade com os requisitos estabelecidos pelo Decreto nº 10.278/2020.</mark>

<mark style="color:red;">Portanto,</mark> <mark style="color:red;"></mark><mark style="color:red;">**não se deve realizar qualquer tipo de manipulação ou edição no documento**</mark><mark style="color:red;">, sob pena de invalidação do processo e perda da conformidade normativa.</mark>
{% endhint %}

### Ativar novo fluxo

Utilizado para ativar um novo fluxo com o registro selecionado já associado a ele. Esse ícone só será habilitado se o cliente possuir o serviço ArqFlow contratado. Será aberta a tela “[Ativar Novo Fluxo](localizacao-simples.md#ativar-novo-fluxo)”.

<figure><img src="../.gitbook/assets/doc41.png" alt=""><figcaption></figcaption></figure>

### Download em Massa

O Download em Massa permite que, ao localizar um documento que possua arquivos associados a ele, seja feito o download de todos esses documentos de uma só vez.

<figure><img src="../.gitbook/assets/doc42.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

É possível solicitar um download em massa de documentos por árvore organizacional ou por lista do cliente, no campo “Tipo de Download”.

<figure><img src="../.gitbook/assets/doc43.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Depois de selecionar o tipo de download é preciso selecionar os itens que se deseja incluir no download em massa e o tipo de arquivo que será gerado, que pode ser arquivo único em formato PDF ou de todos os arquivos em uma pasta ZIP. No arquivo PDF podem também ser incluídas capas separadoras por tipo documental.

{% hint style="warning" %}
<mark style="color:orange;">**O arquivo gerado será disponibilizado em até 24 horas, dependendo do tamanho do arquivo solicitado, no menu**</mark> [<mark style="color:orange;">**Download em Massa**</mark>](download-em-massa.md)<mark style="color:orange;">**. Os arquivos selecionados para download em massa devem totalizar até 500MB.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/doc44.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Ao lado de cada registro outros ícones podem ser exibidos. São eles:

<figure><img src="../.gitbook/assets/doc45.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Endereço:** Passando o mouse sobre esse ícone será possível ver o código do endereço onde aquele documento está alocado na unidade Arquivar ou na estrutura própria do cliente (documentos de Guarda Interna ou Guarda Terceirizada).

<figure><img src="../.gitbook/assets/doc46.png" alt=""><figcaption></figcaption></figure>

**Editar:** Clicando neste botão será possível editar os campos indexadores do documento.

**Download:** Clicando neste ícone será possível realizar o download dos arquivos do documento selecionado.

{% hint style="danger" %}
Se ao tentar realizar o download do arquivo for exibida a mensagem **"Não foi possível carregar o plug-in"**, siga os passos abaixo para ajustar as configurações do navegador:

1. Acesse as configurações do navegador.
2. Navegue até **Privacidade e Segurança**.
3. Localize a opção **Documentos em PDF** ou similar.
4. Em **Comportamento Padrão**, selecione a opção **Fazer o download dos PDFs**.

Essa configuração é padrão do navegador e pode interferir na visualização ou no download dos arquivos PDF, sendo necessário ajustá-la para corrigir o problema.
{% endhint %}
