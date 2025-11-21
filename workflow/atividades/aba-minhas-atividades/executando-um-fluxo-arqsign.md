# ➡️ Executando um fluxo - ArqSign

## Envio dos Documentos para Assinatura via ArqSign

Quando o fluxo atinge uma etapa do tipo **ArqSign**, a aplicação realiza automaticamente a integração com a plataforma de assinaturas, enviando os documentos que foram **marcados para assinatura**.

Neste momento, é gerada uma **tarefa de acompanhamento** no workflow, destinada aos usuários configurados como **responsáveis pela etapa**. A definição desses responsáveis é feita na aba **Configuração** da própria etapa ArqSign.

## Atividade de Acompanhamento

Enquanto o fluxo ainda **não avança para a próxima etapa**, a tarefa de acompanhamento permanece ativa e acessível para os usuários definidos como **responsáveis pelo acompanhamento** da etapa.

Durante esse período, os usuários podem **monitorar o andamento do processo de assinatura** e, conforme as permissões configuradas na etapa, realizar **ações manuais**, tais como:

* **Cancelar o processo** enviado para o ArqSign;
* **Reenviar o processo**, caso o link de assinatura tenha expirado antes da conclusão;
* **Editar signatários** que ainda não assinaram.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (2).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### Interação com Token e Signatários

Na aba **Configurações** da etapa ArqSign, existem dois campos que controlam a possibilidade de interação com processos em andamento:

* **Permitir atualizar token ArqSign expirado**
* **Permitir editar signatários que não assinaram**

As permissões se comportam da seguinte forma:

* **Se ambos os campos estiverem marcados**, o responsável pela tarefa poderá, **em uma única ação**, editar os signatários pendentes e **atualizar o token expirado** dos mesmos, garantindo continuidade ao processo de assinatura.
* **Se apenas o campo “Permitir editar signatários que não assinaram” estiver marcado**, o usuário poderá realizar edições **somente enquanto o processo estiver dentro do prazo de validade**. Caso o token expire, nenhuma ação será possível, a menos que a permissão de atualização também esteja ativada.

### Ação: Cancelar Processo ArqSign

Esta ação estará disponível **somente se** a etapa do tipo ArqSign possuir marcada a configuração **“Permitir cancelar o processo ArqSign”**.

Ao clicar no botão **Cancelar Processo**, o sistema:

* Verifica se todas as obrigatoriedades da tarefa estão preenchidas;
* Exibe uma **mensagem de confirmação** solicitando que o usuário valide a intenção de cancelamento.

Caso o usuário **não confirme**, a mensagem será fechada e a tela da tarefa permanecerá inalterada.\
Caso o usuário **confirme**, o ArqGED, via integração, realiza o **cancelamento do processo na plataforma ArqSign** e **avança o fluxo conforme o conector configurado para a opção “Cancelado”**.

### Ação: Reenviar Processo ArqSign

O botão **Reenviar Processo** será exibido **somente quando**:

* A etapa do tipo ArqSign possuir a configuração **“Permitir atualizar token ArqSign expirado”**;
* E o processo de assinatura estiver **vencido**.

Se a opção **“Obrigar comentário antes desta ação”** estiver marcada, o sistema irá apresentar uma **tooltip** indicando a obrigatoriedade de comentário, e se ele **já foi registrado ou não**.

Ao acionar esta ação, o sistema exibe a **modal de Reenvio de Processo**, permitindo ao responsável reenviar o processo de assinatura aos signatários com tokens expirados.

### Ação: Editar e Reenviar Processo ArqSign

O botão **Editar e Reenviar Processo** será exibido **somente se** a etapa possuir a configuração **“Permitir editar signatários que não assinaram”**.

Importante:

* Quando **somente esta opção estiver marcada**, a ação estará disponível **apenas enquanto o processo não estiver vencido**;
* Caso o processo esteja vencido e **não exista permissão para atualização do token**, o botão **não será exibido**.

Se a opção **“Obrigar comentário antes desta ação”** estiver habilitada, o sistema também apresentará uma **tooltip de obrigatoriedade**, informando se já foi preenchida.

Ao clicar nesta ação, o sistema exibirá a **modal “Editar e Reenviar Processo”**, onde será possível ajustar os dados dos signatários que ainda não assinaram e reenviar o processo à plataforma ArqSign.

<figure><img src="../../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Ícone: Anexos

O **ícone de Anexos** estará visível na tarefa de acompanhamento e tem o objetivo de exibir todos os documentos envolvidos no processo de assinatura via ArqSign.

Ao acionar o ícone, o sistema **exibe uma modal com os documentos relacionados** à etapa, conforme o tipo e status da tarefa.

#### Etapas diferentes de ArqSign

Quando o fluxo possui **etapas comuns com obrigatoriedade de seleção de documentos para assinatura**, esta modal será usada para visualizar, ordenar e confirmar os documentos marcados para envio ao ArqSign.

{% hint style="warning" %}
O sistema **permite selecionar até 25 arquivos** para envio ao ArqSign, somando:

* Anexos do fluxo;
* Anexos dos registros;
* Modelo do fluxo.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### Etapas do tipo ArqSign

<figure><img src="../../../.gitbook/assets/image (6) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### Documentos Assinados

<figure><img src="../../../.gitbook/assets/image (7).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Ícone: Processo ArqSign

O **ícone de Processo ArqSign** permite visualizar informações detalhadas sobre o andamento da etapa de assinatura eletrônica integrada ao fluxo.

#### Acompanhamento do Processo

Ao acionar o ícone, o sistema **exibe uma modal com as informações completas do processo de assinaturas**, permitindo que o usuário acompanhe:

* O **status geral do processo** (em andamento, concluído, cancelado, expirado etc.);
* A **ordem dos signatários** e suas respectivas ações (se já assinaram, recusaram ou estão pendentes);
* A **data e hora de cada movimentação** dentro do processo;
* Quais documentos estão sendo assinados e seu status individual.

Essa modal facilita o acompanhamento técnico do processo e é fundamental para decisões relacionadas ao reenvio, cancelamento ou edição dos signatários, conforme permissões da etapa.

#### **Processo de assinaturas em andamento**

<figure><img src="../../../.gitbook/assets/image (8).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### Processo de assinaturas concluído

<figure><img src="../../../.gitbook/assets/image (9).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

## Recebimento dos Dados via Webhook ArqSign

Sempre que houver uma interação relevante no processo de assinatura, a plataforma ArqSign envia, via **webhook**, os dados de acompanhamento para o ArqGED. Estes dados são processados automaticamente pelo sistema para garantir o acompanhamento em tempo real por parte dos responsáveis definidos na tarefa.

As situações que disparam o envio de dados via webhook incluem:

✅ Processo assinado por algum signatário;

❌ Processo com falha de envio;

🚫 Processo recusado por algum signatário;

🛑 Processo cancelado pelo remetente;

⏳ Processo expirado.

Ao receber os dados de **conclusão**, o ArqGED realiza o tratamento e avança automaticamente o fluxo com base nas configurações dos **conectores de saída** definidos na etapa do tipo ArqSign. Os possíveis encaminhamentos são:

➡️ Avançar se **Concluído**: Todos os signatários concluíram a assinatura.

➡️ Avançar se **Alguém recusou assinar**: Um ou mais signatários recusaram a assinatura.

➡️ Avançar se **Cancelado**: Processo cancelado no ArqSign ou na tarefa de acompanhamento do ArqGED.

➡️ Avançar se **Link de assinatura expirado**: Opção opcional, ativada apenas se não houver tratamento manual de reenvio na etapa do tipo ArqSign.

## Anexos – Dados da Assinatura

Após a conclusão do processo de assinatura, o sistema disponibiliza a visualização e o download do registro de assinaturas vinculadas a cada documento assinado.

Para isso, o usuário deve acionar o **ícone de assinatura** localizado ao lado do nome do arquivo/documento. Ao clicar no ícone, o sistema abre a **modal de assinaturas**, onde é possível:

* Visualizar os dados de cada signatário;
* Consultar data e hora das assinaturas;
* Baixar o **registro completo de assinaturas**.

Essa funcionalidade é essencial para fins de auditoria, comprovação legal e rastreabilidade dos documentos assinados digitalmente via ArqSign.

### Workflow > Atividade > Anexos Visualizar dados de assinaturas

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Visualizar documento > Aba Arquivos

<figure><img src="../../../.gitbook/assets/image (11).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Baixar Registro de Assinaturas

Na **modal de dados de assinaturas**, o usuário tem a opção de realizar o download do certificado com o registro de assinaturas do documento.

Para isso, basta acionar o botão **\[Baixar Certificado de Assinaturas]**.\
Ao clicar, o sistema ArqGED realiza automaticamente o **download do arquivo** contendo o histórico completo das assinaturas realizadas via ArqSign.

Este certificado pode ser utilizado como comprovante legal da integridade e autenticidade das assinaturas digitais realizadas.
