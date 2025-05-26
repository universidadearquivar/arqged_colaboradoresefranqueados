---
hidden: true
---

# 🔹 ArqSign

A aba **ArqSign** é exibida automaticamente entre as abas **Dados Gerais** e **Fluxograma** após o salvamento dos dados gerais de um desenho de fluxo que possui um serviço do tipo **ArqSign Plataforma**.

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

Nesta seção, o usuário pode definir a **mensagem padrão** que será enviada aos destinatários do processo de assinatura que **não possuem mensagens personalizadas configuradas individualmente**.

A mensagem padrão é composta por:

1. **Título da mensagem padrão para todos os signatários** _(opcional)_\
   Campo de texto utilizado para informar o **título** da notificação enviada aos signatários.
2. **Texto da mensagem padrão para todos os signatários** _(opcional)_\
   Campo de texto utilizado para redigir o **corpo da mensagem padrão** que acompanhará a solicitação de assinatura.

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

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
Essa informação é **somente para organização interna** e **não será enviada ao ArqSIGN**.
{% endhint %}

**5. Prazo para disparar notificações via ArqGED** _(opcional)_\
Define o tempo de tolerância até o envio da notificação de atraso.

<figure><img src="../../.gitbook/assets/image (285).png" alt=""><figcaption></figcaption></figure>

O tempo em "Minuto(s)", "Hora(s)", caso o Cliente possua horário de trabalho marcado como referência "para Usuários Externos", serão contados considerando dia e horário de trabalho. Caso contrário serão considerados minutos e horas corridas a partir do início.

&#x20;O tempo em "Dia(s) Útil(eis) ", caso o Cliente possua horário de trabalho para definição das folgas e calendário para definição de feriados como referência "para Usuários Externos", serão contados somente dias úteis. Caso contrário, serão considerados dias corridos.

{% hint style="success" %}
O tempo definido neste campo será usado na aplicação como referência para definição de atraso para a assinatura de cada signatário. Os gatilhos para os envios das mensagens serão configurados no componente ArqSIGN do fluxograma. Desta forma será necessário controlar o início de assinatura de cada signatário: Se o documento não tiver ordem de assinatura, o início de assinatura é o momento do envio do processo, mas para os signatários com ordem de assinatura, o início de assinatura é o horário de conclusão da assinatura de ordem anterior.

Este campo deve ser preenchido somente se o Cliente precisar notificar alguém em relação ao atraso da assinatura por parte de algum signatário.
{% endhint %}

