# 🟩 Explorar

O objetivo do menu Explorar é localizar documentos por meio de uma busca feita pela árvore documental do cliente. Para isso, é necessário selecionar o cliente e definir se deseja visualizar a estrutura documental agrupada pela árvore organizacional ou pelas listas do cliente.

<figure><img src="../../.gitbook/assets/documento5.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## **Visualizar estrutura documental**

{% embed url="https://app.supademo.com/demo/cmaxwhd4z7p9fho3r1wz4sajj" %}

### **Por Árvore Organizacional**

Ao escolher visualizar a estrutura documental agrupada pela Árvore Organizacional, para localizar um documento será preciso explorar todos os níveis da árvore do cliente até chegar ao último, que enfim exibirá o tipo documental desejado. Esse tipo de busca só é recomendado se o usuário souber exatamente em que nível da árvore se encontra o documento que está buscando. Depois de localizar o tipo documental, na parte direita da tela serão exibidos os arquivos existentes.

<figure><img src="../../.gitbook/assets/doc20.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

### **Por Listas**

Também é possível localizar utilizando-se as listas criadas para o cliente no menu [Lista > Criar lista](../../lista/criar-listas.md). Neste caso serão exibidas todas as listas criadas para o cliente no lado esquerda da tela. Para localizar o tipo documental será preciso explorar todos os níveis da lista até chegar ao tipo documental desejado.

<figure><img src="../../.gitbook/assets/doc21.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Visualizar documentos

{% embed url="https://app.supademo.com/demo/cmaxy411l7r6sho3rssvwqkfp" %}

No campo “Visualizar documentos agrupados por” é possível escolher entre visualizar os documentos agrupados por metadados ou por arquivos.

### **Por metadados**

A visualização por metadados permite que sejam exibidas as informações de indexação de todos os registros.

<figure><img src="../../.gitbook/assets/doc22.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

### **Por arquivos**

Na visualização por arquivos são exibidos apenas registros que possuem arquivos anexados. Neste caso, são exibidas as informações desses arquivos.

<figure><img src="../../.gitbook/assets/doc23.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Ícones da tela Explorar

<figure><img src="../../.gitbook/assets/doc24.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

### Adicionar Registro ![](<../../.gitbook/assets/image (128).png>)

Ao selecionar o tipo documento desejado será possível adicionar um novo documento a ele, clicando no ícone “Adicionar”. Será aberta a tela [Documento > Cadastrar](../cadastrar.md) para o cadastro do novo registro.

### Editar ![](<../../.gitbook/assets/image (129).png>)

Utilizado para editar informações do registro que estiver selecionado. Será aberta a mesma tela mostrada em [Documento > Cadastrar](../cadastrar.md).

### Visualizar ![](<../../.gitbook/assets/image (130).png>)

Utilizado para visualizar as informações do registro que estiver selecionado. Será aberta a mesma tela mostrada em [Documento > Cadastrar](../cadastrar.md).

### Excluir ![](<../../.gitbook/assets/image (131).png>)

Utilizado para excluir o registro que estiver selecionado.

### Download do documento ![](<../../.gitbook/assets/image (132).png>)

Utilizado para realizar o download dos arquivos associados ao registro selecionado. Se não houver arquivos anexados ao registro, não é possível realizar o download.

Se selecionado mais de um registro para download com arquivos anexados, será possível escolher entre realizar o download em massa de todos os arquivos em um PDF único, em um arquivo ZIP com vários arquivos ou como arquivos em PDF separados por tamanho do documento (de acordo com o tamanho escolhido pelo usuário). O resultado das solicitações de download em massa feitas nessa tela será disponibilizado na tela [Documento > Download em Massa](../download-em-massa.md).

<div><figure><img src="../../.gitbook/assets/doc25.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure> <figure><img src="../../.gitbook/assets/doc26.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure></div>

{% hint style="danger" %}
Se ao tentar realizar o download do arquivo for exibida a mensagem **"Não foi possível carregar o plug-in"**, siga os passos abaixo para ajustar as configurações do navegador:

1. Acesse as configurações do navegador.
2. Navegue até **Privacidade e Segurança**.
3. Localize a opção **Documentos em PDF** ou similar.
4. Em **Comportamento Padrão**, selecione a opção **Fazer o download dos PDFs**.

Essa configuração é padrão do navegador e pode interferir na visualização ou no download dos arquivos PDF, sendo necessário ajustá-la para corrigir o problema.
{% endhint %}

### Upload de documento ![](<../../.gitbook/assets/image (133).png>)

Utilizado para fazer o upload de um arquivo para associá-lo ao registro selecionado, ou seja, anexar um arquivo àquele documento. Deverá ser informada a versão e o nome do arquivo que está sendo anexado.

<figure><img src="../../.gitbook/assets/doc27.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

### Assinatura ![](<../../.gitbook/assets/image (134).png>)

Se o cliente possuir o serviço de Assinatura Digital contratado, será exibido o ícone “Assinatura”. Será possível realizar a assinatura em lote dos arquivos selecionados no grid de todos os arquivos dos resultados da pesquisa realizada (sendo limitado a 300 arquivos por vez).

<figure><img src="../../.gitbook/assets/doc28.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">Para assinatura de documentos tratados em conformidade com o Decreto 10.278, os arquivos que atingirem 300MB ou mais deverão ser tratados com o fracionamento em partes sequenciais devidamente nomeadas. Caso haja numeração preexistente, como o número de atendimento, sugerimos utilizar essa identificação no nome do arquivo para facilitar a organização e a futura localização do registro no ArqGED.</mark>

<mark style="color:orange;">**Exemplo:**</mark>

<mark style="color:orange;">Prontuário de atendimento nº 100, o fracionamento correto do arquivo deve ser:</mark>

<mark style="color:orange;">100 parte 01/03.pdf</mark>

<mark style="color:orange;">100 parte 02/03.pdf</mark>

<mark style="color:orange;">100 parte 03/03.pdf</mark>

<mark style="color:orange;">Esse procedimento visa otimizar o manuseio e a entrega dos arquivos, evitando possíveis dificuldades no processo de assinatura do acervo.</mark>
{% endhint %}

### Configurar colunas da tela ![](<../../.gitbook/assets/image (135).png>)

As colunas exibidas na tela podem ser escolhidas de acordo com o que se deseja que seja exibido. No campo “Colunas com os dados de identificação do documento”, é possível escolher as colunas que serão exibidas ao se realizar a busca de arquivos do tipo documental selecionado. No campo à esquerda são exibidas as colunas disponíveis e no campo à direita são mostradas as colunas selecionadas que serão exibidas.

<figure><img src="../../.gitbook/assets/doc29.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Para exibir uma coluna, selecione-a no campo à esquerda e clique no ícone “>>”. Para retirar uma coluna da visualização, basta selecioná-la no campo à direita e clicar no ícone “<<”. Para alterar a ordem em que as colunas são exibidas utilize as setas para cima e para baixo.

<figure><img src="../../.gitbook/assets/doc30.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

### Digitalizar documento ![](<../../.gitbook/assets/image (136).png>)

Ao clicar neste ícone o usuário será direcionado para o [módulo ArqScan](modulo-arqscan.md) para que seja feita a indexação do registro selecionado.

<figure><img src="../../.gitbook/assets/doc31.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

### Reservar documento ![](<../../.gitbook/assets/image (137).png>)

Este ícone só será habilitado se houver documento físico associado ao registro selecionado, ou seja, documentos que tenham sido castrados como de “Guarda Interna” ou “Guarda Terceirizada” na tela [Documento > Cadastrar](../cadastrar.md). Neste caso será possível [solicitar a consulta](../../solicitacao/consulta.md) aos documentos físicos por meio deste ícone.

### Reservar caixa ![](<../../.gitbook/assets/image (139).png>)

Este ícone só será habilitado se houver caixa física de documentos associada ao registro selecionado. Neste caso será possível [solicitar a consulta](../../solicitacao/consulta.md) aos documentos das caixas por meio deste ícone.

### Reservar subcaixa ![](<../../.gitbook/assets/image (138).png>)

Este ícone só será habilitado se houver subcaixa física de documentos associada ao registro selecionado. Neste caso será possível [solicitar a consulta](../../solicitacao/consulta.md) aos documentos das subcaixas por meio deste ícone.

### Ativar novo fluxo ![](<../../.gitbook/assets/image (140).png>)

Utilizado para ativar um novo fluxo com o registro selecionado já associado a ele. Esse ícone só será habilitado se o cliente possuir o serviço ArqFlow contratado. Será aberta a tela “[Ativar Novo Fluxo](./#ativar-novo-fluxo)”.

<figure><img src="../../.gitbook/assets/doc32.png" alt=""><figcaption></figcaption></figure>

### Compartilhar ![](<../../.gitbook/assets/image (6) (1) (1) (1).png>)

Permite realizar o compartilhamento do registro selecionado com pessoas externas ao ArqGED, por meio de uma URL gerada para envio por e-mail. É possível definir se essa URL terá acesso por tempo indeterminado ou se terá uma data determinada de validade.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

### Descompartilhar ![](<../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png>)

Utilizado para cessar o acesso aos links gerados por meio do botão “Compartilhar” e enviados por e-mail a usuários externos. Neste caso as pessoas que clicarem no link não conseguirão mais acessar o documento compartilhado.

### Como compartilhar um documento quando ele já possui um compartilhamento em execução

Neste caso, o processo seria realizar o "Descompartilhamento", conforme orientação anterior e realizar novamente o compartilhamento, porém, neste caso os usuários com acesso ao documento perderiam o a link, ou seja o acesso seria cessado.

Para que os compartilhamentos anteriores não sejam perdidos, o ideal é ao clicar no ícone de "Descompartilhar"

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

O link é novamente habilitado na tela, juntamente com o campo de envio por e-mail:

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Neste momento basta copiar o mesmo link ou enviar por e-mail aos novos usuários, sem efetivar o "Descopartilhamento" ou seja, o cancelamento do compartilhamento anterior, sendo mantido os acessos dos usuários anteriores.

Caso opte pelo "Descompartilhamento" clicando no botão disponível, os usuários externos que até então, utilizavam o link, perderão o acesso ao documento.

### Carregar mais 1000 registros ![](<../../.gitbook/assets/image (143).png>)

Por padrão, a tela Explorar exibe no máximo 1000 registros ao se realizar uma busca. Para exibir mais que essa quantidade de registros, deve-se clicar neste ícone.

### Capturar Certificado ![](<../../.gitbook/assets/image (144).png>)

Utilizado para capturar os certificados digitais de arquivos assinados digitalmente. Se houver certificados digitais utilizados para assinatura do registro será possível visualizar as informações desses certificados.

<figure><img src="../../.gitbook/assets/doc34.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

### Filtrar dados de registro

É possível também filtrar os resultados exibidos utilizando o campo “Filtrar dados de registro”.

<figure><img src="../../.gitbook/assets/doc35.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>
