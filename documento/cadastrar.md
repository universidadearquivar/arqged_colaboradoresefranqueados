# 🟩 Cadastrar

Neste menu são cadastrados todos os documentos do cliente. Os documentos cadastrados podem ser do tipo:

* **Eletrônicos:** Documentos eletrônicos não possuem cópia física, podendo ser consultados a qualquer momento no próprio sistema ArqGED.
* **Guarda Interna:** Documentos de Guarda Interna possuem versão física e estão armazenados com o cliente, em sua própria estrutura.
* **Guarda Terceirizada:** Documentos de Guarda Terceirizada possuem versão física e estão armazenados na unidade Arquivar que atende ao cliente. Para que sejam consultados é preciso realizar uma solicitação pelo menu [Solicitação > Consulta](../solicitacao/consulta.md).

<figure><img src="../.gitbook/assets/documento1.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Independentemente do tipo de documento, no momento do cadastro é importante e necessário informar à qual cliente e unidade aquele documento que está sendo criado pertence.

***

## Cadastro de Documento

{% embed url="https://app.supademo.com/demo/cmawkqwny6maqho3r0zu6aby6" %}

### Eletrônico

Depois de selecionar o Universo de Trabalho e a Árvore Organizacional será solicitado preencher os metadados do documento. Os campos de preenchimento aqui foram aqueles anteriormente criados nos menus[ Árvore Documental > Campos Customizados](../arvore-documental/campo-customizado.md) e [Lista](../lista/criar-listas.md).

<figure><img src="../.gitbook/assets/documento2.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Caso necessário também é possível anexar arquivos ao documento que está sendo criado. Para isso, selecione o documento desejado e informe um nome para o arquivo, que será anexado ao documento que está sendo cadastrado.

<figure><img src="../.gitbook/assets/documento3.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Serão exibidos na parte direita da tela os campos indexadores do documento para preenchimento. Os campos exibidos aqui são aqueles definidos anteriormente para o tipo documental escolhido na árvore organizacional do cliente.

<figure><img src="../.gitbook/assets/documento4.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Se tiver sido definido que a lista de campos não permite indexação no momento do cadastro do documento, alguns campos serão desabilitados porque só será permitida a inclusão de informações já existentes na lista. Essa configuração é feita anteriormente no menu**</mark> [<mark style="color:blue;">**Lista > Criar Listas**</mark>](../lista/criar-listas.md)<mark style="color:orange;">**, no campo “Permitir a inclusão durante a indexação”. Esses dados preexistentes devem ser cadastrados via API ou por meio de planilha de importação.**</mark>
{% endhint %}

Os campos azuis são do tipo lista e os campos pretos são campos customizados. Depois de preencher os dados do documento que está sendo cadastrado, clique em “Salvar”.

<figure><img src="../.gitbook/assets/doc01.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Depois de salvar o documento serão habilitadas as abas “Dados Cadastrais”, “Arquivos”, “Histórico” e “Workflow”.

<figure><img src="../.gitbook/assets/doc02.png" alt=""><figcaption></figcaption></figure>

***

### Guarda Interna

Documentos de Guarda Interna são aqueles documentos que existem fisicamente e estão alocados na própria estrutura do cliente, ou seja, em um galpão, sala, armário ou outra estrutura que empresa possua para arquivar seus documentos.

Depois de selecionar o cliente e a unidade, informe se será criada uma caixa ou pasta para armazenar o documento que está sendo criado ou se será utilizada uma caixa ou pasta já existente.

<figure><img src="../.gitbook/assets/doc03.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Se selecionada a opção “Não”, será utilizada uma caixa ou pasta já existente. Neste caso, no lado direito da tela será exibido o campo “Nº Caixa ou Pasta”, para que seja informado o número da caixa onde o documento que está sendo cadastrado será armazenado.

<figure><img src="../.gitbook/assets/doc04.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Se for ser criada uma nova caixa, deverá ser escolhido o “Tipo de Caixa ou Pasta”.

{% hint style="warning" %}
<mark style="color:orange;">**Os tipos de caixa ou pasta exibidos aqui são aqueles criados anteriormente para o cliente no menu**</mark> [**Caixa ou Pasta > Criar**](../caixa-ou-pasta/criar.md)<mark style="color:orange;">**.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/doc05.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Depois de selecionar o Universo de Trabalho e a Árvore Organizacional, caso necessário também será possível anexar arquivos ao documento que está sendo criado. Para isso, selecione o documento desejado e informe um nome para o arquivo, que será anexado ao documento que está sendo cadastrado.

<figure><img src="../.gitbook/assets/doc07.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Serão exibidos na parte direita da tela os campos indexadores do documento para preenchimento. Os campos exibidos aqui são aqueles definidos anteriormente para o tipo documental escolhido na árvore organizacional do cliente anteriormente criados nos menus [Árvore Documental > Campos Customizados](../arvore-documental/campo-customizado.md) e [Lista](../lista/).

{% hint style="warning" %}
<mark style="color:orange;">**Se tiver sido definido que a lista de campos não permite indexação no momento do cadastro do documento, alguns campos serão desabilitados porque só será permitida a inclusão de informações já existentes na lista. Essa configuração é feita anteriormente no menu**</mark> [<mark style="color:blue;">**Lista > Criar Listas**</mark>](../lista/criar-listas.md)<mark style="color:orange;">**, no campo “Permitir a inclusão durante a indexação”. Esses dados preexistentes devem ser cadastrados via API ou por meio de planilha de importação.**</mark>
{% endhint %}

Os campos azuis são do tipo lista e os campos pretos são campos customizados. Depois de preencher os dados do documento que está sendo cadastrado, clique em “Salvar”.

<figure><img src="../.gitbook/assets/doc06.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Depois de salvar o documento serão habilitadas as abas “Dados Cadastrais”, “Arquivos”, “Histórico” e “Workflow”.

<figure><img src="../.gitbook/assets/doc02.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

### Guarda Terceirizada

Documentos de Guarda Interna são aqueles documentos que existem fisicamente e estão alocados no galpão da unidade Arquivar que atende aquele cliente.

Depois de selecionar o cliente, é preciso informar, no lado direito da tela o “Nº de Caixa ou Pasta”. Isso significa que obrigatoriamente, antes de iniciar o cadastro de um documento, é necessário criar as caixas ou pastas que irão armazenar os documentos daquele cliente no menu [Caixa ou Pasta > Criar](../caixa-ou-pasta/criar.md).

<figure><img src="../.gitbook/assets/doc08.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Se tiver sido definido anteriormente que a caia ou pasta informada possui subcaixa ou código provisório, estes também deverão ser informados.**</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/doc09.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Depois de selecionar o Universo de Trabalho e a Árvore Organizacional, caso necessário também será possível anexar arquivos ao documento que está sendo criado. Para isso, selecione o documento desejado e informe um nome para o arquivo, que será anexado ao documento que está sendo cadastrado.

<figure><img src="../.gitbook/assets/doc11.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Serão exibidos na parte direita da tela os campos indexadores do documento para preenchimento. Os campos exibidos aqui são aqueles definidos anteriormente para o tipo documental escolhido na árvore organizacional do cliente anteriormente criados nos menus [Árvore Documental > Campos Customizados](../arvore-documental/ordenacao-campos.md) e [Lista](../lista/).

{% hint style="warning" %}
<mark style="color:orange;">**Se tiver sido definido que a lista de campos não permite indexação no momento do cadastro do documento, alguns campos serão desabilitados porque só será permitida a inclusão de informações já existentes na lista. Essa configuração é feita anteriormente no menu**</mark> [<mark style="color:blue;">**Lista > Criar Listas**</mark>](../lista/criar-listas.md)<mark style="color:orange;">**, no campo “Permitir a inclusão durante a indexação”. Esses dados preexistentes devem ser cadastrados via API ou por meio de planilha de importação.**</mark>
{% endhint %}

Os campos azuis são do tipo lista e os campos pretos são campos customizados. Depois de preencher os dados do documento que está sendo cadastrado, clique em “Salvar”.

<figure><img src="../.gitbook/assets/doc10.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Depois de salvar o documento serão habilitadas as abas “Dados Cadastrais”, “Arquivos”, “Histórico” e “Workflow”.

<figure><img src="../.gitbook/assets/doc02.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Aba Dados Cadastrais

{% embed url="https://app.supademo.com/demo/cmawud1zb6w9sho3rgvagk75c" %}

Nesta aba são exibidas as informações cadastradas do documento e o código gerado para ele, que pode ser visualizado no campo “Código do Documento”. No caso de documentos de Guarda Interna e Guarda Terceirizada será exibido também o campo “Nº Caixa ou Pasta”, que mostrará o número da caixa ou pasta em que o documento está armazenado e o ícone do status da caixa (em indexação ou armazenada) e informações sobre a tabela de temporalidade do documento e destinação final, se houver.

<figure><img src="../.gitbook/assets/doc12.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Serão habilitados também os botões:

**Enviar para Caixa:** Utilizado quando é necessário criar uma versão física do documento eletrônico e enviar para ser armazenada em uma caixa que esteja alocada na unidade Arquivar ou no próprio espaço do cliente.

{% hint style="warning" %}
<mark style="color:orange;">A função</mark> <mark style="color:orange;">**"Enviar para a Caixa"**</mark> <mark style="color:orange;">é utilizado também quando necessário transferir um registro/documento para outra caixa, como por exemplo, a indexação foi realizada de forma indevida na caixa 1010, sendo que fisicamente o documento encontra-se na caixa 1020. Para alterar, basta realizar o envio do documento para a caixa correta.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/doc16.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Novo Registro:** Utilizado para iniciar o registro de um novo documento.

**Excluir:** Utilizado para excluir o documento cadastrado.

**Editar:** Utilizado para alterar as informações do documento cadastrado.

<figure><img src="../.gitbook/assets/doc13.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Aba Arquivo

Caso algum arquivo tenha sido anexado ao documento, nesta aba ele será exibido. Os ícones exibidos sinalizam o tipo de arquivo (PDF, Word, Excel etc.), se possui OCR ou não, se foi assinado digitalmente ou não e se foi compartilhado ou não.

<figure><img src="../.gitbook/assets/doc14.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Clicando nos ícones será possível realizar as seguintes ações em relação a esse arquivo:

<figure><img src="../.gitbook/assets/doc15.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

* **Editar:** Utilizado para editar o nome do documento e numerar a sua versão.
* **Excluir:** Utilizado para excluir o documento que estiver selecionado.
* **Download:** Utilizado para baixar o documento selecionado. O documento será aberto para visualização e download.
* **Upload:** Utilizado para inserir um novo anexo ao documento.
* **Assinar:** Utilizado para assinar os documentos. O usuário pode escolher entre assinar todos os documentos apresentados ou assinar apenas os que estiverem selecionados em verde no grid.
* **OCR:** Habilita o serviço de realização de OCR (Optical Character Recognition, ou Reconhecimento de Caractere Óptico) das páginas do documento anexado. Essa opção só está disponível caso o cliente tenha do serviço ArqOCR contratado.
* **Compartilhar:** Permite realizar o compartilhamento do registro selecionado com pessoas externas ao ArqGED, por meio de uma URL gerada para envio por e-mail. É possível definir se essa URL terá acesso por tempo indeterminado ou se terá uma data determinada de validade.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

* **Descompartilhar:** Utilizado para cessar o acesso aos links gerados por meio do botão “Compartilhar” e enviados por e-mail a usuários externos. Neste caso as pessoas que clicarem no link não conseguirão mais acessar o documento compartilhado.
* **Como compartilhar um documento quando ele já possui um compartilhamento em execução:** Neste caso, o processo seria realizar o "Descompartilhamento", conforme orientação anterior e realizar novamente o compartilhamento, porém, neste caso os usuários com acesso ao documento perderiam o a link, ou seja o acesso seria cessado.

Para que os compartilhamentos anteriores não sejam perdidos, o ideal é ao clicar no ícone de "Descompartilhar"

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

O link é novamente habilitado na tela, juntamente com o campo de envio por e-mail:

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Neste momento basta copiar o mesmo link ou enviar por e-mail aos novos usuários, sem efetivar o "Descopartilhamento" ou seja, o cancelamento do compartilhamento anterior, sendo mantido os acessos dos usuários anteriores.

Caso opte pelo "Descompartilhamento" clicando no botão disponível, os usuários externos que até então, utilizavam o link, perderão o acesso ao documento.

* **Capturar certificado:** Quando se faz o upload de um documento que esteja assinado digitalmente, clicando neste ícone será possível extrair e visualizar as informações sobre o certificado digital utilizado para a assinatura. Quando o documento for assinado no próprio GED o certificado de assinaturas ficará disponível automaticamente.

***

## Aba Histórico

Nesta aba será possível visualizar o histórico de todas as solicitações de consulta e devoluções do documento (de Guarda Interna ou de Guarda Terceirizada) realizadas pelo cliente.

São exibidas as informações de número do documento, número do pedido, código da caixa onde o documento está armazenado, processo (consulta ou devolução), status, se foi localizado ou recebido, nome do solicitante, nome do atendente e data do fechamento ou recebimento.

<figure><img src="../.gitbook/assets/doc17.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Aba Workflow

Nesta aba é possível verificar todos os fluxos aos quais o documento está associado, com informações do código do fluxo, nome do processo, etapa atual em que se encontra, responsável atual, data de ativação do fluxo, status do fluxo e situação.

<figure><img src="../.gitbook/assets/doc18.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Clicando nos ícones será possível realizar as seguintes ações em relação ao documento:

<figure><img src="../.gitbook/assets/doc19.png" alt=""><figcaption></figcaption></figure>

* **Ativar novo fluxo:** Utilizado para ativar um novo fluxo já com o documento associado a ele.
* **Desassociar:** Utilizado para desvincular o registro selecionado do fluxo. O documento continua existindo no sistema mas não terá mais relação com o fluxo.
* **Visualizar desenho:** Utilizado para visualizar o desenho do fluxo ao qual o documento está associado.
* **Comentário:** Utilizado para verificar os comentários feitos no fluxo ao qual o documento está associado.
* **Anexos:** Utilizado para visualizar os anexos do fluxo ao qual o documento está associado.
* **Formulário:** Utilizado para visualizar o formulário do fluxo ao qual o documento está associado.
* **Modelo Documento:** Utilizado para visualizar o modelo PDF se existir algum associado ao fluxo.
