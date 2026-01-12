# 🔹 Módulo ArqScan

## Pré-requisitos para a utilização do ArqScan

Para que o módulo ArqScan funcione corretamente é necessária a instalação de um scanner e do driver que fará a comunicação entre o sistema e o aparelho de scanner. Além disso, é preciso também instalar o aplicativo ArqClient na máquina do usuário, utilizado para a comunicação entre a máquina do usuário, scanners e tokens.

{% hint style="warning" %}
<mark style="color:orange;">**Deve ser instalado na máquina do usuário o driver correspondente ao seu aparelho de scanner. Verifique a marca e modelo do scanner e busque o driver correspondente a ele.**</mark>
{% endhint %}

### Instalando/Atualizando o ArqClient

{% @supademo/embed demoId="cmaz9sd2691w7ho3r9ablcwsj" url="https://app.supademo.com/demo/cmaz9sd2691w7ho3r9ablcwsj" %}

O ArqClient precisa ser instalado na máquina do usuário como requisito para utilização das funcionalidades do ArqSCAN e ArqSIGN (Assinatura Digital) no software ArqGED. O software ArqClient possui duas funções:

* Realizar a comunicação entre o ArqSCAN e o driver de scanner (para o uso do ArqSCAN).
* Realizar a comunicação entre o ArqGED e certificados de assinatura digital, seja via tokens, certificados instalados na máquina ou cartões inteligentes (para uso da assinatura digital).

Para o funcionamento correto do ArqClient são exigidos os requisitos mínimos abaixo.

* Memória RAM: Mínimo 4 GB
* Processador: Dual Core, 2 GHz ou Superior.
* Sistema Operacional: Windows 10, ou superior

1\. Para realizar o download e instalação do aplicativo “ArqClient” na máquina onde será utilizada a assinatura digital, acesse o site [**https://downloads.arquivar.com/**](https://downloads.arquivar.com/).

<figure><img src="../../../.gitbook/assets/image (50).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

2\. Em “Instaladores”, clique no link para o arquivo de instalação para utilização no ambiente de Produção.

<figure><img src="../../../.gitbook/assets/arqscan02.png" alt=""><figcaption></figcaption></figure>

3\. Salve o arquivo ZIP na máquina. Em seguida, clique com o botão direito do mouse e extraia os arquivos utilizando o programa "WinRAR". Selecione a opção "Extrair para...".

<figure><img src="../../../.gitbook/assets/image (7) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

4. Abra a pasta criada na extração dos arquivos e clique duas vezes sobre o arquivo de instalação.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

5\. Clique em “Avançar” nas próximas telas até que o status de instalação seja concluído.

<figure><img src="../../../.gitbook/assets/arqscan04.png" alt=""><figcaption></figcaption></figure>

6\. Clique em “Fechar” para concluir a instalação.

<figure><img src="../../../.gitbook/assets/arqscan05.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
[<mark style="color:blue;">**Clique aqui**</mark>](https://view.genial.ly/65269e7884447000117c67f7) <mark style="color:orange;">**e acesse o conteúdo completo sobre o aplicativo ArqClient.**</mark>
{% endhint %}

O acesso ao módulo ArqScan deve ser feito na tela [Documento > Explorar](./), clicando no ícone “Digitalizar”.

<figure><img src="../../../.gitbook/assets/arqscan06.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="danger" %}
<mark style="color:red;">Os aplicativos da Arquivar Addin / ArqIndex / ArqClient podem apresentar erros durante o uso, por falta de pacotes específicos no desktop.</mark>

<mark style="color:red;">Estes erros são solucionados após a instalação de pacotes .Net e VC Redist."</mark>

<mark style="color:red;">Veja abaixo um exemplo de erro deste tipo:</mark>

<img src="https://arquivar.gitbook.io/~gitbook/image?url=https%3A%2F%2F1023047207-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FtM1xGMYoU6wC7tnUUXEo%252Fuploads%252FiKWqsB9T52cwxnfPd6fl%252Fimage.png%3Falt%3Dmedia%26token%3D1edf8ffd-7b46-4e76-bc88-e5a3daf9d14c&#x26;width=300&#x26;dpr=4&#x26;quality=100&#x26;sign=1a85218b&#x26;sv=1" alt="" data-size="original">

<mark style="color:red;">Clique nos links abaixo para baixar os instaladores para estes pacotes. É importante utilizar sempre a versão mais atual para instalação.</mark>

1. [<mark style="color:red;">**VC Redist.**</mark>](https://learn.microsoft.com/pt-br/cpp/windows/latest-supported-vc-redist?view=msvc-170#latest-microsoft-visual-c-redistributable-version)
2. [<mark style="color:red;">**.Net**</mark>](https://dotnet.microsoft.com/pt-br/download/dotnet/3.1)

<mark style="color:blue;">Estes erros são apresentados com maior frequência em Notebooks e Máquinas Virtuais.</mark>

<mark style="color:red;">Em caso de dúvidas, entre em contato com nosso suporte pelo ArqAtende.</mark>
{% endhint %}

***

## Digitalizando documentos

Para iniciar a digitalização de um documento, insira-o no aparelho de scanner e na tela do ArqScan clique no ícone “Digitalizar”. As páginas serão digitalizadas e exibidas na tela.

<figure><img src="../../../.gitbook/assets/arqscan07.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (346).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Ao clicar em uma imagem digitalizada será possível expandi-la para visualização. Na tela de visualização da imagem também será possível racioná-la para a direita e esquerda, girá-la 180° e mover a imagem. Na paginação na parte inferior será possível navegar entre as imagens digitalizadas.

<figure><img src="../../../.gitbook/assets/image (348).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Voltando à tela inicial do ArqScan, clicando com o botão direito do mouse sobre uma imagem será possível:

**Excluir:** Exclui a página selecionada.

<figure><img src="../../../.gitbook/assets/image (350).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Girar:** Girar a página selecionada em 90° à direita ou à esquerda e em 180°.

<figure><img src="../../../.gitbook/assets/image (351).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Ordenação:** Alterar a ordenação da imagem selecionada, enviando a para o início, para o fim ou para uma posição específica entre as páginas digitalizadas.

<figure><img src="../../../.gitbook/assets/image (352).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (353).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Clicando no ícone “Visualização” é possível alterar a quantidade de imagens exibidas no grid.&#x20;

<figure><img src="../../../.gitbook/assets/image (354).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

O ícone de três barras é utilizado para ocultar ou mostra o menu lateral.

<figure><img src="../../../.gitbook/assets/image (355).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

***

{% hint style="danger" %}
<mark style="color:red;">Pode acontecer em alguns casos, ao abrir o ArqScan para continuidade de um processo aparecer a seguinte mensagem de erro:</mark>

<mark style="color:red;">**Erro! O total de imagens .tif na pasta "C:\temp\ScannerPath" é diferente do total de imagens na pasta "C:\temp\ScannerPath\Thumbnails", verifique a relação de arquivos existentes nestas pastas.**</mark>

<mark style="color:red;">Esse erro pode ser ocasionado por vários fatores, dentre eles podemos destacar:</mark>

<mark style="color:red;">• Falha na conexão com a internet o que pode corromper a transmissão dos dados para o sistema;</mark>

<mark style="color:red;">• Falha no HD da maquina física que pode corromper a gravação dos dados;</mark>

<mark style="color:red;">• Estouro na memoria RAM que pode não suportar a transmissão dos dados.</mark>

<mark style="color:red;">Para sanar o problema, é necessário acessar as pastas onde ficam os arquivos temporários e apagar as imagens, desta forma o ArqScan voltará a funcionar corretamente.</mark>

<mark style="color:red;">Pastas que devem ser verificadas:</mark>

<mark style="color:red;">**C:\temp\ScannerPath**</mark>

<mark style="color:red;">**C:\temp\ScannerPath\Thumbnails**</mark>
{% endhint %}

***

## Realizando a indexação de documentos

Para iniciar a indexação, selecione as páginas que deseja indexar. É possível selecionar mais de uma página por vez, mantendo a tecla Ctrl pressionada e selecionando as páginas que deseja indexar.

<figure><img src="../../../.gitbook/assets/image (357).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Na área “Indexadores” será exibido o cliente selecionado anteriormente em [Documento > Explorar](./). Selecione o Universo de Trabalho, a Árvore Organizacional e o Tipo de Documento (Eletrônico, Guarda Interna ou Guarda Terceirizada). O campo “Unidade” será preenchido automaticamente com a unidade que atende o cliente selecionado.

<figure><img src="../../../.gitbook/assets/arqscan17.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Depois de realizar a seleção serão exibidos os campos indexadores para preenchimento. Esses campos são aqueles definidos anteriormente para o tipo documental que estiver sendo indexado. O preenchimento desses campos funciona da mesma forma que no [cadastro de documentos](../cadastrar.md).

<figure><img src="../../../.gitbook/assets/arqscan19.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Caso tenha sido escolhido o tipo de documento “Guarda Interna” será preciso informar se será feita a criação de uma nova caixa. Se não for criada será preciso informar o número da caixa e subcaixa (se houver) à qual o documento será associado. Se escolhido o tipo de documento de “Guarda Terceirizada” será obrigatório informar o número da caixa e subcaixa (se houver).

<figure><img src="../../../.gitbook/assets/arqscan18.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Na área “Imagem” é possível nomear as imagens manualmente ou selecionar a opção “Gerar Nome Automaticamente”.

<figure><img src="../../../.gitbook/assets/image (359).png" alt=""><figcaption></figcaption></figure>

No campo “Driver”, selecione o driver correspondente ao scanner que está sendo utilizado. Clicando no ícone “Configurações” serão exibidas as configurações do scanner e do driver.

<figure><img src="../../../.gitbook/assets/arqscan14.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**As configurações do scanner são definidas pelo fabricante do aparelho e variam de acordo com a marca e modelo utilizado. Para maiores informações sobre essas configurações, procure o site ou documentação do fabricante do aparelho de scanner que estiver utilizando.**</mark>
{% endhint %}

<figure><img src="../../../.gitbook/assets/arqscan15.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

No campo “OCR” é possível selecionar a opção “Gerar PDF pesquisável”. Essa opção permite que as imagens do PDF que for gerado serão pesquisáveis por meio do módulo ArqOCR.

{% hint style="warning" %}
<mark style="color:orange;">**Para utilizar essa opção é necessário que o cliente possua o módulo ArqOCR contratado.**</mark>
{% endhint %}

<figure><img src="../../../.gitbook/assets/arqscan21.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Na área “Assinatura” é possível assinar digitalmente o documento que for gerado. Para isso será preciso possuir um certificado digital instalado na máquina. Se houver mais de um certificado instalado, basta selecionar aquele que deseja utilizar.

<figure><img src="../../../.gitbook/assets/image (358).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Na área “Workflow” é possível ativar um novo fluxo associando os documentos digitalizados a ele. Para isso, é preciso selecionar o processo, inserir as observações (se houver) e informar se a ativação será imediata ou deverá ser feita em uma data e horários agendados.

Também é possível associar os documentos digitalizados a um fluxo já existente. Para isso é preciso informar o número do fluxo do cliente que esteja ativo e em execução e inserir observações (se houver).

<figure><img src="../../../.gitbook/assets/arqscan23.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Ao selecionar as opções “Manter Metadados” e “Manter Dados” selecionadas, os dados e configurações feitas na indexação serão mantidos para o próximo registro.

<figure><img src="../../../.gitbook/assets/arqscan24.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Depois de concluir as configurações de indexação, clique no ícone “Upload”. Para fazer o upload de páginas específicas selecione a opção “Fazer upload somente dos arquivos selecionados”. Confirme o envio das imagens. Se tiver sido definido que será feita a assinatura dos documentos, será solicitada a senha do certificado digital escolhido.

<figure><img src="../../../.gitbook/assets/arqscan25.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

As páginas selecionadas serão indexadas e sumirão da tela de digitalização. Para visualizá-las, retorne à tela [Documento > Explorar](./) e localize o tipo documental do cliente ao qual o registro foi associado. Quando localizar, selecione-o e clique no ícone “Download do documento” para visualizar o PDF gerado com as páginas digitalizadas.

<figure><img src="../../../.gitbook/assets/arqscan26.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>
