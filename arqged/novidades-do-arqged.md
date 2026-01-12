---
icon: lightbulb-exclamation-on
---

# Novidades do ArqGED

## Workflow - Dez/2025

02/12 > Fluxo de trabalho da Nova Tela de Atividades

A página de Atividades agora possui uma opção de exibição em " [Lista](https://manual.arquivar.com/manual-arqged-or-clientes/arqged/workflow/atividades/aba-minhas-atividades#botao-dados-listagem) ", permitindo que as informações sejam apresentadas de forma mais simples e organizada para o usuário conectado. [Clique para mais detalhes.](https://manual.arquivar.com/manual-arqged-or-clientes/arqged/workflow/atividades/aba-minhas-atividades/executando-um-fluxo-1#visualizacao-listagem)

02/12 > Configuração do Layout de Tarefas Internas

Durante a [configuração da etapa](https://manual.arquivar.com/manual-arqged-or-clientes/arqged/workflow/desenho-do-fluxo/aba-fluxograma#aba-layout-tarefa-interna) , agora é possível definir com mais detalhes quais áreas devem ser visíveis e/ou obrigatórias para o usuário durante a execução do fluxo. Isso torna o processo mais limpo, fluido e reduz o número de cliques necessários.

02/12 > Permissão de visualização padrão da Tela de Atividades

Agora é possível definir, nas permissões do usuário, se a exibição padrão da Tela de Atividades deve ser em "Listagem" ou "Dados", [clique para mais detalhes.](https://manual.arquivar.com/manual-arqged-or-clientes/arqged/administracao/usuarios#aba-perfil)&#x20;

***

## Compartilhamento de Arquivos via API - Set/2025

02/09 > Novos Serviços de Compartilhamento de Arquivos via API

**APIs de Compartilhamento**

Foram adicionados três novos serviços na[ **API** ](https://manual.arquivar.com/manual-arqged-or-clientes/arqged/integracoes/api)relacionados ao compartilhamento de arquivos já cadastrados em documentos no ArqGED:

1. **POST - Gerar link de compartilhamento**
   * Permite compartilhar arquivos de um documento já existente.
   * Obrigatório: ID do documento e ID do cliente (no cabeçalho da requisição).
   * Opcional: ID de imagem específica e prazo de compartilhamento.
   * Se não for informado o ID da imagem, todos os arquivos do documento serão compartilhados.
   * O retorno inclui ID da imagem, descrição, nome do arquivo e link de compartilhamento.
2. **GET - Consultar links de compartilhamento**
   * Retorna todos os links de compartilhamento de arquivos associados a um documento.
   * Obrigatório: ID do documento e ID do cliente (no cabeçalho).
   * Não há opção de consultar apenas um arquivo específico – a consulta sempre retorna todos os arquivos compartilhados do documento.
3. **DEL - Deletar link de compartilhamento**
   * Permite remover (de forma lógica) o compartilhamento de arquivos.
   * Obrigatório: ID do documento e ID do cliente (no cabeçalho).
   * Opcional: ID da imagem.
   * Caso não seja informado o ID da imagem, todos os compartilhamentos do documento serão removidos.
   * A exclusão não é física: é registrada apenas uma data de expiração para o compartilhamento.

**⚙️ Padrões gerais da API**

* Todas as requisições exigem Subscription Key e token de autorização.
* IDs de documentos, clientes e imagens podem ser obtidos pelos serviços já existentes de busca na API.
