---
hidden: true
---

# 🔹 ArqSign

A aba **ArqSign** é exibida automaticamente entre as abas **Dados Gerais** e **Fluxograma** após o salvamento dos dados gerais de um desenho de fluxo que possui um serviço do tipo **ArqSign Plataforma**.

Essa aba permite configurar as integrações com a plataforma ArqSign para envio de documentos para assinatura digital durante a execução do fluxo.

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
