# 🔹 ArqSign

{% embed url="https://app.supademo.com/demo/cmbus472jfardsn1r128xpsat" %}

A aba **ArqSign** é exibida automaticamente entre as abas **Dados Gerais** e **Fluxograma** após o salvamento dos dados gerais de um desenho de fluxo que possui um serviço do tipo **Assinador ArqSign**.

Essa aba permite configurar as integrações com a plataforma ArqSign para envio de documentos para assinatura digital durante a execução do fluxo.

<figure><img src="../../.gitbook/assets/image (273).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### Sobre as configurações da aba ArqSign

* Cada desenho de fluxo pode conter **uma ou mais configurações** de integração com o ArqSign.
* Essas configurações serão posteriormente **associadas às etapas do tipo ArqSign**, definindo os pontos do fluxo nos quais os documentos serão enviados para assinatura.
* Os dados cadastrados incluem as informações necessárias para o envio do processo à plataforma ArqSign.

#### Ações disponíveis

As ações abaixo são habilitadas apenas para fluxos com status **"Em Elaboração"** ou **"Inativo"**, e que **ainda não foram versionados**:

1.  **Adicionar**

    Abre uma nova aba no navegador com o formulário para inclusão de nova configuração de ArqSign.
2.  **Editar**

    Requer que uma configuração esteja selecionada no GRID. Abre a configuração selecionada em modo de edição, em nova aba do navegador.
3.  **Visualizar**

    Habilitado após a seleção de uma configuração no GRID. Abre a configuração selecionada em modo de visualização, em nova aba do navegador.
4.  **Excluir**

    Requer seleção de uma configuração no GRID. Exclui a configuração selecionada de ArqSign.

#### Observação

Ao excluir uma configuração de ArqSign que esteja vinculada a uma etapa do tipo ArqSign, o sistema **remove automaticamente essa referência**.\
Na próxima validação do fluxo, será exibida uma **lista de etapas do tipo ArqSign sem a configuração associada**, exigindo novo vínculo para a continuidade do processo.

## Tela de Configuração da Aba ArqSign

Na tela de **Configuração ArqSIGN**, o usuário deve informar os dados necessários para o envio do processo de assinaturas de documentos por meio da integração com a plataforma **ArqSIGN**.

A configuração é composta por três seções principais:

* **Configurações Gerais ArqSIGN**
* **Mensagem Padrão ArqSIGN**
* **Destinatários ArqSIGN**

## Configurações Gerais ArqSIGN

{% embed url="https://app.supademo.com/demo/cmbux43rbffi4sn1rkjs98sym" %}

A seção **Configurações Gerais** define os parâmetros operacionais do processo de assinatura. Veja abaixo o detalhamento de cada campo:

### Campos obrigatórios e opcionais

**1. IdConta – Conta** _(somente leitura)_\
Exibe o **nome e o ID da conta ArqSIGN** vinculada ao serviço selecionado.

**2. Pasta** _(obrigatório)_\
Campo para seleção da pasta no ArqSign onde o processo será criado.

* Ao clicar, o sistema abrirá um modal com a lista de pastas disponíveis na conta.

<figure><img src="../../.gitbook/assets/image (277).png" alt="" width="285"><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**3. Responsável** _(obrigatório)_\
Campo para seleção do responsável pelo processo de assinaturas.

* O sistema listará todos os **usuários ativos da conta ArqSign**.

**4. Nome do Processo** _(obrigatório)_\
Campo de texto onde o usuário deve informar o **nome do processo** que será criado na plataforma ArqSign.

<figure><img src="../../.gitbook/assets/image (274).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Prazos e lembretes

**1. Lembrete**\
Define o intervalo em **dias** para envio automático de lembretes aos signatários.

* Ex: enviar novo alerta de assinatura a cada 3 dias.

**2. Renovação**\
Define o intervalo em **meses** para o sistema ArqSign notificar o remetente sobre a necessidade de renovar o documento.

**3. Expiração**\
Define o número de **dias até a expiração automática** do documento após o envio.

**4. Expiração – Lembrete**\
Define com quantos dias de antecedência será enviado um **aviso da expiração**.

<figure><img src="../../.gitbook/assets/image (275).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Configurações avançadas

**Obrigar leitura do documento**\
<sub>Campo de marcação opcional.</sub>

* Se marcado, o ArqSign exigirá que o usuário **leia o documento antes de assinar**.
* Se desmarcado, o usuário poderá assinar sem abrir o conteúdo.

**Substituir o arquivo original no ArqGED pelo assinado via ArqSign**\
<sub>Campo de marcação opcional.</sub>

* Define se o documento assinado pelo ArqSign **deve substituir automaticamente** o arquivo original armazenado no ArqGED.

**Gerar QRCode de acesso ao documento**\
<sub>Campo de marcação opcional.</sub>

* Se marcado, ao final do processo, o sistema gerará um **QRCode de acesso individual** para cada documento assinado.
* O link será visível diretamente na plataforma ArqSign.

<figure><img src="../../.gitbook/assets/image (276).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

## Mensagem Padrão ArqSign

{% embed url="https://app.supademo.com/demo/cmbv15lxvfkfmsn1rj22gn6wh" %}

Nesta seção, o usuário pode definir a **mensagem padrão** que será enviada aos destinatários do processo de assinatura que **não possuem mensagens personalizadas configuradas individualmente**.

A mensagem padrão é composta por:

1. **Título da mensagem padrão para todos os signatários** _(opcional)_\
   Campo de texto utilizado para informar o **título** da notificação enviada aos signatários.
2. **Texto da mensagem padrão para todos os signatários** _(opcional)_\
   Campo de texto utilizado para redigir o **corpo da mensagem padrão** que acompanhará a solicitação de assinatura.

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="warning" %}
Caso um destinatário tenha uma mensagem personalizada configurada, essa substituirá a mensagem padrão.
{% endhint %}

## Destinatários ArqSign

Nesta seção, o usuário configura os **signatários que participarão do processo de assinaturas eletrônicas** por meio da plataforma ArqSign.

É necessário preencher os campos que definem quem assinará os documentos, como serão enviados os convites de assinatura e quais regras devem ser seguidas durante a execução do fluxo.

### Informações Gerais

<figure><img src="../../.gitbook/assets/image (281).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**Importante:**</mark>\ <mark style="color:orange;">As assinaturas serão</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**posicionadas automaticamente**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">ao final de cada documento pelo ArqSIGN.</mark>

<mark style="color:orange;">O ArqGED</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**não define a posição visual da assinatura**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">nos arquivos.</mark>
{% endhint %}

**1. Usar ordem de assinatura** _(opcional)_\
Campo de marcação utilizado para indicar se os signatários devem seguir uma **ordem definida de assinatura**.

Ao ativar essa opção, será exibido o campo “Ordem” em cada card de signatário.

<figure><img src="../../.gitbook/assets/image (280).png" alt=""><figcaption></figcaption></figure>

**2. Ordem** _(obrigatório se a opção anterior estiver marcada)_\
Define a sequência de assinatura. O sistema insere a numeração automaticamente (1, 2, 3...), mas o usuário pode editar conforme necessário.

<figure><img src="../../.gitbook/assets/image (279).png" alt=""><figcaption></figcaption></figure>

**3. Ícone da lixeira**\
Permite excluir o card de signatário.

<figure><img src="../../.gitbook/assets/image (282).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
O sistema exige que **ao menos um card permaneça na tela**.
{% endhint %}

### Dados do signatário

**4. Tipo de destinatário** _(obrigatório)_\
Campo para nomear o tipo de signatário (ex: Cliente, Funcionário, Diretor, Testemunha).

{% hint style="info" %}
Essa informação é **somente para organização interna** e **não será enviada ao ArqSign**.
{% endhint %}

**5. Prazo para disparar notificações via ArqGED** _(opcional)_\
Define o tempo de tolerância até o envio da notificação de atraso.

<figure><img src="../../.gitbook/assets/image (285).png" alt=""><figcaption></figcaption></figure>

O tempo em "Minuto(s)", "Hora(s)", caso o Cliente possua horário de trabalho marcado como referência "para Usuários Externos", serão contados considerando dia e horário de trabalho. Caso contrário serão considerados minutos e horas corridas a partir do início.

&#x20;O tempo em "Dia(s) Útil(eis) ", caso o Cliente possua horário de trabalho para definição das folgas e calendário para definição de feriados como referência "para Usuários Externos", serão contados somente dias úteis. Caso contrário, serão considerados dias corridos.

{% hint style="success" %}
O tempo definido neste campo será usado na aplicação como referência para definição de atraso para a assinatura de cada signatário. Os gatilhos para os envios das mensagens serão configurados no componente ArqSign do fluxograma. Desta forma será necessário controlar o início de assinatura de cada signatário: Se o documento não tiver ordem de assinatura, o início de assinatura é o momento do envio do processo, mas para os signatários com ordem de assinatura, o início de assinatura é o horário de conclusão da assinatura de ordem anterior.

Este campo deve ser preenchido somente se o Cliente precisar notificar alguém em relação ao atraso da assinatura por parte de algum signatário.
{% endhint %}

### Informações do formulário

<figure><img src="../../.gitbook/assets/image (286).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**6. Campo onde extrair o nome** _(obrigatório)_\
Campo para definir de onde será extraído o nome do signatário no formulário.

Serão listados apenas **campos do tipo texto**.

**7. Enviar por** _(obrigatório)_\
Define o meio de envio do processo ao destinatário. Opções:

* E-mail
* WhatsApp (exibido somente se o serviço ArqSign possuir subserviço WhatsApp)

{% hint style="info" %}
A forma de envio determina o tipo de campo permitido em “Campo onde extrair o e-mail ou telefone”.
{% endhint %}

**8. Campo onde extrair o e-mail ou telefone** _(obrigatório)_\
Define o campo do formulário onde será extraído o o e-mail ou telefone do destinatário.

{% hint style="info" %}
O sistema só aceita campos compatíveis com o canal de envio (e-mail ou telefone).\
Não é permitido repetir a mesma referência de campo em destinatários com mesma ordem ou sem ordem.
{% endhint %}

### Configurações de assinatura

**9. Este destinatário irá:** _(obrigatório)_\
Define o tipo de participação do destinatário no processo. Opções:

* Assinar Online como Pessoa Física
* Assinar Online como Pessoa Jurídica
* Receber uma Cópia

<figure><img src="../../.gitbook/assets/image (287).png" alt=""><figcaption></figcaption></figure>

Ao selecionar “Receber uma Cópia”, as opções de assinatura serão desmarcadas automaticamente.

Se forem selecionados ambas as opções, para pessoa física e jurídica, a assinatura terá de ser feita pelo mesmo signatário como os dois papeis distintos, conforme marcação.&#x20;

**10. Assinatura de Pessoa Física como** _(opcional)_\
Disponível apenas se o item "_Este destinatário irá"_ “Assinar Online como Pessoa Física”.

<figure><img src="../../.gitbook/assets/image (288).png" alt=""><figcaption></figcaption></figure>

**11. Assinatura de Pessoa Jurídica como** _(opcional)_\
Disponível apenas se o item "_Este destinatário irá"_ for “Assinar Online como Pessoa Jurídica”.

<figure><img src="../../.gitbook/assets/image (289).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Ao clicar nestes campos (10 e 11), o sistema lista os papeis de signatário da conta no ArqSign, assim como o valor default da conta marcado (caso exista valor default). Embora possa ter um valor default, ele pode ser desmarcado e não será obrigatório que haja alguma marcação.
{% endhint %}

**12. Tipo de Assinatura** _(obrigatório)_\
Define o tipo de assinatura permitida. Opções:

* Assinatura Eletrônica
* Certificado Digital Pessoal do Tipo ICP-Brasil
* Certificado Digital Pessoal Todos os Tipos

<figure><img src="../../.gitbook/assets/image (290).png" alt=""><figcaption></figcaption></figure>

**13. Estilo de Assinatura** _(opcional)_\
Define a forma de apresentação da assinatura. Opções:

* Padrão
* Desenho
* Imagem

<figure><img src="../../.gitbook/assets/image (291).png" alt=""><figcaption></figcaption></figure>

**14. Este signatário NÃO precisa existir para enviar ao ArqSign** _(opcional)_\
Permite que o processo seja criado mesmo se os dados do signatário estiverem ausentes.

<figure><img src="../../.gitbook/assets/image (293).png" alt=""><figcaption></figcaption></figure>

Desta forma, estando a flag marcada para algum signatário, quando chegar o momento no fluxo de criar o processo no ArqSign, caso não exista informações de nome e e-mail/telefone para o signatário, o processo será criado sem ele.

{% hint style="success" %}
<mark style="color:green;">**Exemplo de Uso:**</mark> Isso pode ser usado para processos em que em determinado momento há 1 testemunha e em outro há 2. Então a configuração da segunda testemunha seria opcional.
{% endhint %}

### Colapse: Configurações Adicionais

O colapse **Configurações Adicionais** estará disponível **somente** para destinatários cuja opção **“Este destinatário irá”** esteja configurada como **Assinatura Online** (Pessoa Física ou Jurídica).

<figure><img src="../../.gitbook/assets/image (294).png" alt=""><figcaption></figcaption></figure>

Ao expandir esse colapse, o sistema apresenta **abas complementares de configuração** para o signatário selecionado. Todas as abas são opcionais.

As abas disponíveis são:

* **Dados Cadastrais**
* **Anexos**
* **Mensagem**
* **Código de Segurança**

<figure><img src="../../.gitbook/assets/image (295).png" alt=""><figcaption></figcaption></figure>

### Ações disponíveis na tela

1. **Adicionar Novo Destinatário**\
   Adiciona um novo **card** de signatário à tela.

{% hint style="info" %}
Se o processo estiver utilizando **ordem de assinatura**, o campo **Ordem** do novo card será automaticamente preenchido com o número subsequente ao último card existente.
{% endhint %}

1. **Voltar**\
   Retorna ao **GRID de workflows**, preservando os filtros aplicados anteriormente na tela.
2. **Salvar**\
   Salva as informações preenchidas ou alteradas referentes aos destinatários e suas configurações.

<figure><img src="../../.gitbook/assets/image (297).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
#### Regras de validação obrigatórias

<mark style="color:red;">É obrigatório informar</mark> <mark style="color:red;"></mark><mark style="color:red;">**ao menos um destinatário**</mark> <mark style="color:red;"></mark><mark style="color:red;">com a opção:</mark>

* <mark style="color:red;">**Assinar Online como Pessoa Física**</mark><mark style="color:red;">, ou</mark>
* <mark style="color:red;">**Assinar Online como Pessoa Jurídica**</mark><mark style="color:red;">,</mark>\ <mark style="color:red;">sem que a flag</mark> <mark style="color:red;"></mark><mark style="color:red;">**“Este signatário NÃO precisa existir para enviar ao ArqSIGN”**</mark> <mark style="color:red;"></mark><mark style="color:red;">esteja marcada.</mark>

<mark style="color:red;">**Quando o processo não possui ordem de assinatura:**</mark>

* <mark style="color:red;">Não é permitido selecionar o</mark> <mark style="color:red;"></mark><mark style="color:red;">**mesmo campo do formulário**</mark> <mark style="color:red;"></mark><mark style="color:red;">para múltiplos destinatários.</mark>

<mark style="color:red;">**Quando o processo possui ordem de assinatura:**</mark>

* <mark style="color:red;">Não é permitido repetir o mesmo campo do formulário entre destinatários com a</mark> <mark style="color:red;"></mark><mark style="color:red;">**mesma ordem**</mark><mark style="color:red;">.</mark>
{% endhint %}

## Configurações Adicionais

{% embed url="https://app.supademo.com/demo/cmbv5fpxtfnxosn1r3gd6zvag" %}

### Aba Dados Cadastrais

A aba **Dados Cadastrais** é exibida somente para destinatários que tenham o campo **Tipo de Assinatura** configurado como **Assinatura Eletrônica**.

Essa aba permite configurar os dados de identificação da Pessoa Física ou Jurídica que assinará o documento.

#### **1. Nome da Pessoa Física**

<figure><img src="../../.gitbook/assets/image (298).png" alt=""><figcaption></figcaption></figure>

* **Campo onde extrair o nome a preencher na tela da assinatura** _(opcional)_
  * Permite definir o campo do formulário de onde será extraído o **nome do signatário** para ser pré-preenchido na tela de assinatura.
  * Serão listados apenas campos do tipo **texto**.
  * Este nome será usado para que no momento da assinatura por parte do signatário o nome já venha preenchido na tela de assinatura.
* **Obrigar o preenchimento do nome** _(opcional)_
  * Se marcado, o signatário deverá preencher obrigatoriamente o campo de nome na hora da assinatura.
  * Se desmarcado, o preenchimento será opcional.

#### **2. Documento da Pessoa Física**

<figure><img src="../../.gitbook/assets/image (299).png" alt=""><figcaption></figcaption></figure>

* **Documento** _(obrigatório)_
  * Define o tipo de documento solicitado ao signatário.
  * Valor padrão: **CPF**
  * Outras opções:
    * CNH
    * RG
    * Outro
* **Obrigar o preenchimento do documento** _(opcional)_
  * Se marcado, o signatário deverá obrigatoriamente preencher o campo de documento durante a assinatura.
* **Nome Documento** _(obrigatório se opção “Outro” estiver selecionada)_
  * Define a **campo personalizado** do documento quando a opção "Outro" for selecionada.
* **Formato** _(obrigatório se opção “Outro” estiver selecionada)_
  * Define o tipo de entrada para o campo de documento.
  * Opções:
    * Texto _(valor padrão)_
    * Numérico
* **Quantidade de Caracteres** _(opcional)_
  * Campo numérico para definir o número máximo de caracteres permitidos para o documento.
* **Campo onde extrair o valor para o documento** _(opcional)_
  * Permite definir o campo do formulário de onde será extraído o valor do documento para envio ao ArqSign.
* **Usar valor de documento para validar** _(opcional)_
  * Se marcado, o número extraído será usado para **validação obrigatória**: o processo só será concluído se o signatário informar exatamente o número que foi enviado.
  * Se desmarcado, o número será apenas **pré-preenchido** para facilitar o processo.

{% hint style="warning" %}
Os dados de Pessoa Jurídica, abaixo, somente serão exibidos quando o campo **Este destinatário irá** estiver configurado como **Assinar Online como Pessoa Jurídica**.
{% endhint %}

#### **3. Nome da Pessoa Jurídica**

<figure><img src="../../.gitbook/assets/image (300).png" alt=""><figcaption></figcaption></figure>

* **Campo onde extrair o nome a preencher na tela da assinatura** _(opcional)_
  * Define o campo do formulário de onde será extraído o **nome da empresa** do signatário.
  * Serão listados apenas campos do tipo **texto**.
* **Obrigar o preenchimento do nome** _(opcional)_
  * Se marcado, o preenchimento do nome da empresa será obrigatório no momento da assinatura.

#### **4. Documento da Pessoa Jurídica**

<figure><img src="../../.gitbook/assets/image (301).png" alt=""><figcaption></figcaption></figure>

* **Documento** _(obrigatório)_
  * Define o tipo de documento da empresa.
  * Valor padrão: **CNPJ**
  * Outras opções:
    * Outro
* **Obrigar o preenchimento do documento** _(opcional)_
  * Se marcado, o preenchimento do campo de documento da empresa será obrigatório no momento da assinatura.
* **Nome Documento** _(obrigatório se opção “Outro” estiver selecionada)_
  * Define o **campo personalizado** do documento da empresa.
* **Formato** _(obrigatório se opção “Outro” estiver selecionada)_
  * Opções:
    * Texto _(valor padrão)_
    * Numérico
* **Quantidade de Caracteres** _(opcional)_
  * Campo numérico para limitar o número de caracteres do documento da empresa.
* **Campo onde extrair o valor para o documento** _(opcional)_
  * Define o campo do formulário de onde será extraído o número do documento da empresa.
* **Usar valor de documento para validar** _(opcional)_
  * Se marcado, o número será usado para **validação obrigatória** durante a assinatura.
  * Se desmarcado, será apenas **pré-preenchido automaticamente**.

### Aba Anexos

A aba **Anexos** estará sempre visível para signatários configurados com a opção **Assinatura Online** (Pessoa Física ou Jurídica).

Essa aba permite configurar se o signatário deverá ou poderá enviar documentos durante o processo de assinatura, além de definir como esses anexos serão armazenados e visualizados.

<figure><img src="../../.gitbook/assets/image (302).png" alt=""><figcaption></figcaption></figure>

#### Permitir anexar documentos durante a assinatura

* Campo de marcação **opcional**.
* Se **marcado**, o sistema exibirá campos adicionais para configurar o envio de anexos por parte do signatário.
* Durante a assinatura, o signatário visualizará a opção de **fazer upload de arquivos**.

#### Campos exibidos ao marcar a opção de anexar documentos

* **Armazenar todos os anexos como Anexo do Fluxo** _(opcional)_\
  Define que os arquivos enviados pelos signatários serão armazenados no ArqGED.
* **Nome Anexo** _(obrigatório)_\
  Campo de texto onde o usuário define o **campo** do anexo a ser enviado pelo signatário.&#x20;

{% hint style="danger" %}
O sistema **não permite nomes repetidos** para anexos do mesmo signatário.
{% endhint %}

* **Obrigar o upload do anexo** _(opcional)_
  * Se **marcado**, o upload do anexo será obrigatório para concluir a assinatura.
  * Se **desmarcado**, o campo será exibido, mas o envio será opcional.
* **Permitir a visualização deste anexo por todos os signatários após a assinatura via ArqSign** _(opcional)_
  * Se **marcado**, o anexo ficará **disponível para todos os signatários** após a conclusão do processo de assinatura.
  * Se **desmarcado**, o anexo estará disponível **somente para o remetente**.

{% hint style="warning" %}
<mark style="color:orange;">**Importante:**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">O acesso aos anexos enviados ao ArqGED seguirá o</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**nível de acesso configurado no ArqGED**</mark><mark style="color:orange;">. A opção acima se refere apenas ao comportamento dentro da</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**plataforma ArqSign**</mark><mark style="color:orange;">.</mark>
{% endhint %}

#### Adicionar mais anexos

* O botão **Adicionar Mais Anexos** permite configurar múltiplos campos de upload para o mesmo signatário.
* Ao pressioná-lo, o sistema exibirá novos grupos de campos como:
  * **Nome Anexo 2**
  * **Obrigar o upload do anexo**
  * **Permitir a visualização deste anexo por todos os signatários após a assinatura via ArqSign**

Esse processo pode ser repetido quantas vezes forem necessárias, criando diferentes etapas de envio por parte do mesmo signatário.

#### Aba Mensagem

A aba **Mensagem** estará sempre visível para signatários configurados com a opção **Assinatura Online**.

Essa aba permite configurar uma **mensagem personalizada** para cada signatário, substituindo a mensagem padrão definida na aba **ArqSign**.

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Campos disponíveis

1. **Título** _(opcional)_\
   Campo de texto utilizado para definir um **título personalizado** da mensagem que será enviada ao signatário.
2.  **Mensagem** _(opcional)_\
    Campo de texto para redigir o **conteúdo personalizado da mensagem** enviada ao signatário.



{% hint style="warning" %}
Ao preencher estes campos, o signatário **não receberá** a mensagem padrão definida na aba ArqSign.
{% endhint %}

### Aba Código de Segurança

A aba **Código de Segurança** estará sempre visível para signatários configurados com a opção **Assinatura Online**.

Essa aba permite configurar o envio de um **código de segurança adicional**, que será solicitado ao signatário no momento da assinatura do documento.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Campos disponíveis

* **Campo onde extrair o código de segurança** _(obrigatório se houver envio)_

Campo do formulário de onde será extraído o código de segurança a ser enviado ao signatário. Este campo precisa ser numérico com a configuração de tamanho mínimo e máximo com valor  igual a **"4".**

<figure><img src="../../.gitbook/assets/image (345).png" alt=""><figcaption></figcaption></figure>

* **Enviar código de segurança por** _(obrigatório se houver código)_\
  Campo para selecionar o **meio de envio** do código de segurança.\
  Opções disponíveis:
  * SMS
  * WhatsApp
  * E-mail
  * Não enviar

{% hint style="warning" %}
<mark style="color:orange;">As opções</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**SMS**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">e</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**WhatsApp**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">só estarão disponíveis se o serviço</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**Plataforma ArqSign**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">selecionado no fluxo possuir os respectivos</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**subserviços habilitados**</mark><mark style="color:orange;">.</mark>&#x20;

<mark style="color:orange;">A escolha do meio de envio</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**determina o tipo de campo a ser selecionado**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">no item seguinte:</mark>
{% endhint %}

* Se **E-mail** for selecionado, o campo de origem deverá conter um **endereço de e-mail**.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

* Se **SMS** ou **WhatsApp** forem selecionados, o campo deverá conter um **telefone**.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

* **Campo onde extrair o e-mail ou telefone** _(obrigatório se houver envio)_\
  Campo do formulário de onde será extraído o **contato** (e-mail ou telefone) para envio do código de segurança.
  * O tipo de dado aceito depende da opção selecionada no campo anterior.
* **Reenviar código de segurança** _(exibido apenas para SMS ou WhatsApp)_\
  Se o envio for realizado via **SMS** ou **WhatsApp**, o sistema apresentará a opção de **reenviar o código de segurança** caso necessário.
