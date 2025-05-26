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

### Configurações Gerais ArqSIGN

A seção **Configurações Gerais** define os parâmetros operacionais do processo de assinatura. Veja abaixo o detalhamento de cada campo:

#### Campos obrigatórios e opcionais

1. **IdConta – Conta** _(somente leitura)_\
   Exibe o **nome e o ID da conta ArqSIGN** vinculada ao serviço selecionado.
2.  **Pasta** _(obrigatório)_\
    Campo para seleção da pasta no ArqSIGN onde o processo será criado.

    > Ao clicar, o sistema abrirá um modal com a lista de pastas disponíveis na conta.
3.  **Responsável** _(obrigatório)_\
    Campo para seleção do responsável pelo processo de assinaturas.

    > O sistema listará todos os **usuários ativos da conta ArqSIGN**.
4. **Nome do Processo** _(obrigatório)_\
   Campo de texto onde o usuário deve informar o **nome do processo** que será criado na plataforma ArqSIGN.

#### Prazos e lembretes _(campos opcionais)_

5.  **Lembrete**\
    Define o intervalo em **dias** para envio automático de lembretes aos signatários.

    > Ex: enviar novo alerta de assinatura a cada 3 dias.
6. **Renovação**\
   Define o intervalo em **meses** para o sistema ArqSIGN notificar o remetente sobre a necessidade de renovar o documento.
7. **Expiração**\
   Define o número de **dias até a expiração automática** do documento após o envio.
8. **Expiração – Lembrete**\
   Define com quantos dias de antecedência será enviado um **aviso da expiração**.

#### Configurações avançadas

9. **Obrigar leitura do documento**\
   Campo de marcação opcional.
   * Se marcado, o ArqSIGN exigirá que o usuário **leia o documento antes de assinar**.
   * Se desmarcado, o usuário poderá assinar sem abrir o conteúdo.
10. **Substituir o arquivo original no ArqGED pelo assinado via ArqSIGN**\
    Campo de marcação opcional.

* Define se o documento assinado pelo ArqSIGN **deve substituir automaticamente** o arquivo original armazenado no ArqGED.

11. **Gerar QRCode de acesso ao documento**\
    Campo de marcação opcional.

* Se marcado, ao final do processo, o sistema gerará um **QRCode de acesso individual** para cada documento assinado.
* O link será visível diretamente na plataforma ArqSIGN.
