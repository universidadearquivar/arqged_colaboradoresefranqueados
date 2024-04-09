# 🟩 Dados Cadastrais

No menu Dados Cadastrais são exibidas todas as informações dos clientes da unidade selecionada no campo “Unidade”.&#x20;

<figure><img src="../.gitbook/assets/clientes8.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Dados Cadastrais – Tela inicial&#x20;

**Campo Unidade:** Para exibir as informações de um cliente, selecione a unidade à qual ele pertence se tiver acesso aos clientes de mais de uma unidade.  &#x20;

**Coluna ID:** O número ID é o código do cliente apresentado nas etiquetas das caixas quando o cliente possui serviço de guarda de documentos contratado. &#x20;

**Coluna Nome Fantasia:** Esta coluna exibe o nome fantasia do cliente. É este nome que será exibido ao realizar o cadastro de qualquer serviço no sistema.   &#x20;

**Coluna Razão Social:** Nesta coluna é exibida a razão social do cliente. A razão social é o nome comercial do cliente, ou seja, seu nome jurídico registrado. &#x20;

**Coluna CPF/CNPJ:** Esta coluna exibe o CPF ou CNPJ do cliente. &#x20;

**Coluna Status:** Informa se cliente está ativo, inativo ou bloqueado na plataforma.  &#x20;

<figure><img src="../.gitbook/assets/cliente01.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Ícone Adicionar:** Utilizado para cadastrar um novo cliente. &#x20;

**Ícone Editar:** Utilizado para editar as informações do cliente selecionado. &#x20;

**Ícone Visualizar:** Utilizado para apresentar as informações do cliente.  &#x20;

**Ícone Excluir:** Utilizado para excluir o cliente selecionado. &#x20;

<figure><img src="../.gitbook/assets/cliente02.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Cadastro de Cliente&#x20;

Para cadastrar um cliente, selecione a unidade e clique no ícone “Adicionar”.&#x20;

<figure><img src="../.gitbook/assets/cliente03.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

### Aba Dados Cadastrais&#x20;

Na aba Dados Cadastrais devem ser cadastradas todas as informações do cliente. &#x20;

**ID:** No campo ID atribua um Id para o cliente. Esse Id é o código do cliente apresentado nas etiquetas das caixas quando o cliente possui serviço de guarda de documentos contratado. &#x20;

**Idioma:** Neste campo o usuário deve definir o idioma do cliente, que pode ser Português, Inglês ou Espanhol. &#x20;

{% hint style="warning" %}
<mark style="color:orange;">**A definição do idioma realizada aqui irá interferir no idioma das telas mostradas aos signatários em ações externas de assinatura de documentos do Workflow.**</mark>
{% endhint %}

**Status:** Informe se cliente está ativo, inativo ou bloqueado na plataforma. &#x20;

* _Ativo:_ Utilizado quando o cliente está com a situação regular para uso da plataforma.&#x20;
* _Bloqueado:_ Utilizado quando o cliente está inadimplente e seu acesso precisa ser interrompido temporariamente até que ele regularize sua situação.&#x20;
* _Inativo:_ Utilizado quando o cliente não tem mais acesso ao sistema.&#x20;

**Nome Fantasia:** Informe o nome fantasia do cliente. Este nome será exibido ao realizar o cadastro de qualquer serviço no sistema.   &#x20;

**Razão Social:** Informe a razão social do cliente. A razão social é o nome comercial do cliente, ou seja, seu nome jurídico registrado. &#x20;

<figure><img src="../.gitbook/assets/cliente04.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**CPF/CNPJ:** Informe o CPF do responsável legal pela empresa ou o CNPJ do cliente.&#x20;

**Inscrição estadual e Inscrição municipal:** Informe as inscrições estadual e municipal do cliente, se ele possuir.&#x20;

<figure><img src="../.gitbook/assets/cliente05.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**IP e DNS para acesso à aplicação:** Por meio deste campo é possível limitar o acesso ao sistema à rede do cliente, determinando que o acesso seja realizado apenas pelos IPs cadastrados. Para isso, selecione entre IP ou DNS, informe o endereço desejado e clique no ícone “Adicionar”. Fazendo essa restrição, só será permitido que os usuários do cliente se autentiquem no sistema se estiverem utilizando um dos IPs ou DNS informados neste campo. &#x20;

{% hint style="warning" %}
<mark style="color:orange;">**Essa configuração só funcionará se o IP ou DNS do cliente for fixo. Se for dinâmico (variável a cada acesso) o sistema não conseguirá fazer o bloqueio do acesso do usuário.**</mark>&#x20;
{% endhint %}

<figure><img src="../.gitbook/assets/cliente06.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Opções de layout padrão e Opções de cor padrão:** As definições de layout feitas nestes campos serão aplicadas a todos os usuários do cliente que utilizarem o sistema. Por padrão as opções “Cabeçalho fixo” e “Menu à esquerda fixo” estarão selecionadas, e a cor verde será o padrão do tema, mas as configurações podem ser alteradas de acordo com a necessidade do cliente.&#x20;

<figure><img src="../.gitbook/assets/cliente07.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Geral:** Configurações gerais do sistema. Neste campo pode ser definido se os usuários do cliente poderão alterar o layout escolhido no campo “Opções de layout padrão”. Se marcada essa opção será exibido o ícone de engrenagem no canto direito da tela, para que os usuários do cliente realizem as alterações de layout que desejarem.&#x20;

<figure><img src="../.gitbook/assets/cliente08.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

A opção “Incluir marca d’água nas imagens” inclui uma marca d’água no rodapé de todos os documentos que forem baixados por usuários, exibindo a data, hora e nome do usuário que realizou o download daquele documento. &#x20;

{% hint style="warning" %}
<mark style="color:orange;">**Para que essa opção funcione corretamente, a permissão “Download sem Marca D’água” deve estar desabilitada para os usuários do cliente, na tela**</mark> [<mark style="color:blue;">**Administração > Perfis de Usuários > Permissões.**</mark>](../administracao/perfis-de-usuarios.md)&#x20;
{% endhint %}

{% hint style="danger" %}
<mark style="color:red;">**Não é recomendado que clientes que utilizem Certificado Digital para assinatura de documentos no sistema utilizem essa opção, porque esse tipo de documento não pode ser manipulado. Ao incluir a marca d’água a integridade do documento e as assinaturas são corrompidas, já que essa inclusão é considerada uma alteração do documento original.**</mark>&#x20;
{% endhint %}

Também é possível bloquear um usuário quando ele mais de cinco tentativas de acesso ao sistema sem sucesso, informando usuário ou senha incorretos. Neste caso o usuário só poderá tentar acessar novamente após alguns minutos. &#x20;

<figure><img src="../.gitbook/assets/cliente09.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Logomarca:** Neste campo deve ser feito o upload das logomarcas utilizadas pelo cliente. Pode ser feito o upload de mais de uma logo. Ao realizar o upload de uma logomarca, no campo “Arquivos que serão associados ao registro” deve ser informado um nome para a logo (de preferência, utilize nomes que descrevam como será a utilização). &#x20;

<figure><img src="../.gitbook/assets/cliente10.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Ao salvar, será possível informar se aquela logo é a padrão (exibida nas telas do sistema), e se será utilizada nos rótulos e etiquetas gerados no sistema. Pode ser escolhida mais de uma logo para rótulos e etiquetas. &#x20;

{% hint style="warning" %}
<mark style="color:orange;">**O ideal é que a logomarca padrão seja toda branca, para uma melhor visualização nas telas do sistema. As logos utilizadas em rótulos e etiquetas devem ser pretas ou coloridas, para melhor visualização nos documentos gerados e impressos.**</mark>&#x20;
{% endhint %}

<figure><img src="../.gitbook/assets/cliente11.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Todas as logos acrescentadas são apresentadas no campo “Logomarcas”. Clicando sobre cada uma é possível visualizá-la no campo “Preview logomarca”. &#x20;

<figure><img src="../.gitbook/assets/cliente12.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

**Observação:** Neste campo podem ser adicionadas informações específicas sobre o cliente.&#x20;

***

### Aba Prestadoras de Serviço&#x20;

Nesta aba são cadastradas as unidades que prestam serviço para o cliente. Para adicionar a Unidade Arquivar responsável pelo cliente, selecione-a na lista e clique no ícone “Adicionar”. É possível associar mais de uma Unidade Arquivar ao cliente, se necessário.&#x20;

{% hint style="warning" %}
<mark style="color:orange;">**É necessário realizar a associação da Unidade ao cliente nesta tela para que seja possível cadastrar o contrato do cliente na tela**</mark> [<mark style="color:blue;">**Cliente > Contratos**</mark>](contratos/)<mark style="color:orange;">**.**</mark>&#x20;
{% endhint %}

Para excluir uma associação, selecione a Unidade e clique no ícone “Excluir”.   &#x20;

<figure><img src="../.gitbook/assets/cliente13.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>
