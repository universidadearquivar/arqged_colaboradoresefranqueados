# ▫️ Setembro | 2025

<details>

<summary>02/09 Novos Serviços de Compartilhamento de Arquivos via API</summary>

**APIs de Compartilhamento**

Foram adicionados três novos serviços na[ **API** ](../integracoes/api/)relacionados ao compartilhamento de arquivos já cadastrados em documentos no ArqGED:

1. **Gerar link de compartilhamento**
   * Permite compartilhar arquivos de um documento já existente.
   * Obrigatório: ID do documento e ID do cliente (no cabeçalho da requisição).
   * Opcional: ID de imagem específica e prazo de compartilhamento.
   * Se não for informado o ID da imagem, todos os arquivos do documento serão compartilhados.
   * O retorno inclui ID da imagem, descrição, nome do arquivo e link de compartilhamento.
2. **Consultar links de compartilhamento**
   * Retorna todos os links de compartilhamento de arquivos associados a um documento.
   * Obrigatório: ID do documento e ID do cliente (no cabeçalho).
   * Não há opção de consultar apenas um arquivo específico – a consulta sempre retorna todos os arquivos compartilhados do documento.
3. **Deletar link de compartilhamento**
   * Permite remover (de forma lógica) o compartilhamento de arquivos.
   * Obrigatório: ID do documento e ID do cliente (no cabeçalho).
   * Opcional: ID da imagem.
   * Caso não seja informado o ID da imagem, todos os compartilhamentos do documento serão removidos.
   * A exclusão não é física: é registrada apenas uma data de expiração para o compartilhamento.

#### ⚙️ Padrões gerais da API

* Todas as requisições exigem Subscription Key e token de autorização.
* IDs de documentos, clientes e imagens podem ser obtidos pelos serviços já existentes de busca na API.

</details>
