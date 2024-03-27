# 🔹 Aplicativo ArqIndex

O aplicativo ArqIndex é necessário para o trabalho de digitalização e indexação dos documentos, seja na unidade ou no cliente. Este aplicativo deve ser instalado na máquina que será utilizada como servidor, na qual ocorrerão os processos. &#x20;

## Instalação do aplicativo ArqIndex&#x20;

A instalação do ArqIndex no cliente ou em uma das unidades franqueadas deve ser feita pela Arquivar Master mediante solicitação da própria unidade Arquivar franqueada por meio do ArqAtende.&#x20;

<details>

<summary>Passo a passo para abertura de chamado no ArqAtende</summary>

1. Acesse o site [https://b24-sd3f59.bitrix24.site/Solicitacoesfranquias/](https://b24-sd3f59.bitrix24.site/Solicitacoesfranquias/)&#x20;
2. Preencha os campos apresentados na tela:&#x20;

* _Unidade de Negócios:_ nome da unidade solicitante&#x20;
* _Nome do cliente:_ Se o chamado estiver sendo aberto para a unidade, repita o nome. Se for para um cliente, informe o cliente para quem o chamado será aberto.&#x20;
* _Dados de contato:_ Informe o nome, e-mail e telefone de quem deve receber o retorno do chamado. Essa pessoa precisa ter condições de repassar informações do processo, pois ela poderá ser contata pelos técnicos da Arquivar Master durante a execução do chamado. Se o chamado estiver sendo aberto para um cliente, o contato deverá ser do responsável pelo atendimento àquele cliente dentro da unidade. &#x20;

3. Clique em “Próximo”.&#x20;
4. No campo “Departamento Atendimento Solicitação” informe o departamento que deve receber sua solicitação.&#x20;

</details>

***

### Requisitos mínimos&#x20;

Alguns processos executados pela aplicação ArqIndex podem demandar um alto processamento de máquina, como memória, processador, espaço em disco, tráfego de rede e internet. É importante que seja avaliado cada detalhe do projeto, pois esta máquina é um grande diferencial, levando em consideração a quantidade de documentos digitalizados bem como a qualidade e tamanho dos arquivos. Seguem os requisitos mínimos da máquina que irá receber a instalação do aplicativo ArqIndex:&#x20;

* Processador de quatro núcleos;&#x20;
* 8 GB de memória RAM;&#x20;
* Espaço de armazenamento em disco de acordo com a demanda de processamento, sendo o mínimo de 250 GB. Caso a unidade ou cliente demande um espaço maior de armazenamento, é recomendável utilizar uma máquina de 500 GB ou mais de armazenamento interno.

***

### Instalação

Após de realizar o download do executável de instalação, execute a instalação, selecione o idioma desejado e clique em “OK”. Nas próximas telas, apenas clique em “Próximo” para instalação padrão. &#x20;

<figure><img src="../../.gitbook/assets/app01.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Por padrão, a pasta de destino da instalação sempre será C:\Program Files (x86)\Arquivar\ArqIndex. O usuário pode escolher outra pasta de destino se desejar.&#x20;

<figure><img src="../../.gitbook/assets/app02.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Acesso ao ArqIndex&#x20;

Depois de instalar o aplicativo do ArqIndex, realize o login utilizando o mesmo usuário e senha de acesso ao ArqGED.&#x20;

<figure><img src="../../.gitbook/assets/app03.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Para acessar o ArqIndex o usuário precisa possuir permissão de acesso ao ArqIndex devidamente habilitada na tela**</mark> [<mark style="color:blue;">**Administração > Usuários > Aba Permissões I**</mark>](../../administracao/usuarios.md) <mark style="color:blue;">**> Perfil de acesso: Gestão ArqINDEX**</mark><mark style="color:orange;">**. Um usuário pode possuir apenas permissão de indexação, de configuração do local de trabalho ou de correção do XML, ou pode possuir uma permissão global, que permite o acesso a todos os menus.**</mark>&#x20;

<img src="../../.gitbook/assets/app04.png" alt="" data-size="original">
{% endhint %}

***

## Configurar Parâmetros&#x20;

Após o login é exibida a tela de configuração dos parâmetros para o funcionamento da aplicação.

**Local de Trabalho:** Neste campo são exibidos os [Parâmetros Gerais](parametros-gerais.md) ou o chamado Local de Trabalho, criados no menu [Produção > Configurações > Parâmetros Gerais](parametros-gerais.md). &#x20;

**Local dos Arquivos de Entrada:** Neste campo é informada a pasta onde serão armazenados os arquivos XML e imagens digitalizadas no scanner. É importante que esta pasta esteja compartilhada na rede, pois será utilizada tanto pelo ArqIndex para indexação quanto pelo scanner para digitalização.

**Local dos Arquivos em Processo:** Neste campo é informada a pasta onde serão armazenados os arquivos processados e validados corretamente pelo ArqIndex para indexação. É importante que essa pasta esteja compartilhada na rede, pois será utilizada pelo ArqIndex para indexação dos documentos.

**Local dos Arquivos em Exportação:** Neste campo é informado a pasta onde serão armazenados os arquivos processados, validados e indexados corretamente pelo ArqIndex. É importante que esSa pasta esteja compartilhada na rede, pois será utilizada pelo ArqIndex para exportação dos documentos indexados para o ArqGED.

**HOST/IP:** Este campo é preenchido automaticamente com o endereço da rede onde foi instalada a aplicação ArqIndex.

{% hint style="warning" %}
<mark style="color:orange;">**Após clicar no botão "Salvar" não será mais possível alterar o Local de Trabalho informado, portanto, tenha total certeza de que o endereço informado é o correto.**</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/app05.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Após criadas as pastas para a configuração dos parâmetros, clique sobre cada pasta criada com o botão direito do mouse, selecione Propriedades > Compartilhamento e copie o “Caminho de Rede” conforme o exemplo abaixo. Após copiado, basta colar o caminho no campo correspondente na aplicação ArqIndex. O ideal é que sejam atribuídos às pastas nomes de fácil identificação.

{% hint style="info" %}
<mark style="color:blue;">**EXEMPLO:**</mark>&#x20;

* <mark style="color:blue;">Local dos Arquivos de Entrada: Entrada</mark>
* <mark style="color:blue;">Local dos Arquivos em Processo: Processo</mark>
* <mark style="color:blue;">Local dos Arquivos em Exportação: Exportação</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/app06.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/app07.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

O campo “HOST/IP” é preenchido automaticamente com o endereço de rede onde está instalado o robô do ArqIndex. Clique em “Salvar”.&#x20;

<figure><img src="../../.gitbook/assets/app08.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## &#x20;Processos&#x20;

Nesta tela são iniciadas as etapas do fluxo de indexação do cliente. As etapas mostradas aqui foram definidas anteriormente na tela [Produção > Configurações > Fluxo de Trabalho](fluxo-de-trabalho.md) para o cliente ou unidade.&#x20;

A primeira etapa a ser executada é o “Host das Imagens”, que deverá criar os certificados de segurança da máquina onde o robô está instalado e das máquinas indexadoras. Clique no ícone “Play”.  &#x20;

<figure><img src="../../.gitbook/assets/app10.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Será criada uma pasta com os certificados necessários para a indexação dentro do local onde o aplicativo está instalado (por padrão, a pasta C:\Program Files (x86)\Arquivar\ArqIndex). &#x20;

<figure><img src="../../.gitbook/assets/app09.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Na etapa “Conversão” deve ser definida a quantidade de núcleos do processador que deverão ser dedicados exclusivamente para o processo de conversão dos documentos, que demanda mais recursos da máquina. Depois de realizar essa definição, clique em “Play”.&#x20;

<figure><img src="../../.gitbook/assets/app11.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Ao iniciar o processo de indexação, clique em “Play” em “Todos os processos”. &#x20;

<figure><img src="../../.gitbook/assets/app12.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**O ideal é que a máquina que for receber o robô do ArqIndex seja dedicada exclusivamente a essa função, já que serão consumidos muito espaço de armazenamento e memória pelo aplicativo e permaneça ligada. Caso seja necessário desligar a máquina ou interromper o ArqIndex por algum motivo, retorne a essa tela e clique em “Pause” em “Todos os processos”.**</mark> &#x20;
{% endhint %}
