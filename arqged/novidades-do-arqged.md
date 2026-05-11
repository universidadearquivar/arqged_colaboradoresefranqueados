# 💡 Novidades do ArqGED

**Campo CNPJ - Maio/2026**

<details>

<summary>11/05 - Campo CNPJ Alfanumérico</summary>

Em atendimento a **Instrução Normativa RFB nº 2.229/2024**, que estabelece a adoção do novo formato do CNPJ em modelo alfanumérico (com letras e números), **foram ajustados todos os campos que utilizam essa informação no ArqGED:**

* Cliente > Dados Cadastrais
* Documento > Cadastrar
* Documento > Localização Simples
* Documento > Localização Avançada
* Campos de Lista (Consolidação / Auto-complete / Provisória)
* Workflow
* API

A mudança será aplicada de forma progressiva a partir de julho de 2026 e se aplica apenas para novos cadastros de CNPJ, sem impacto para os números já existentes, portanto não teremos perda nos registros já criados no **ArqGED.**

</details>

**Workflow - Dezembro/2025**

<details>

<summary>02/12 - Nova Tela de Atividades Workflow</summary>

A tela de Atividades agora conta com a opção de visualização em "[Listagem](../workflow/atividades/aba-minhas-atividades/#botao-dados-listagem)", permitindo que as informações sejam exibidas de forma mais simples e organizada para o usuário logado,[ clique para mais detalhes.](../workflow/atividades/aba-minhas-atividades/executando-um-fluxo-1.md#visualizacao-listagem)

</details>

<details>

<summary>02/12 - Configuração de Layout de Tarefa Interna</summary>

Durante a [configuração da etapa](../workflow/desenho-do-fluxo/aba-fluxograma.md#aba-layout-tarefa-interna), agora é possível definir com mais detalhes quais áreas devem ser visíveis e/ou obrigatórias para o usuário durante a execução do fluxo. Isso torna o processo mais limpo, fluido e reduz a quantidade de cliques necessários.

</details>

<details>

<summary>02/12 - Permissão de Visualização padrão da Tela de Atividades</summary>

Agora é possível definir, nas permissões do usuário, se a exibição padrão da Tela de Atividades deve ser em  "Listagem" ou "Dados",  [clique para mais detalhes.](../administracao/usuarios.md#aba-perfil)

</details>

**Compartilhamento de Arquivos via API - Setembro/2025**

<details>

<summary>02/09 - Novos Serviços de Compartilhamento de Arquivos via API</summary>

**APIs de Compartilhamento**

Foram adicionados três novos serviços na[ **API** ](../integracoes/api/)relacionados ao compartilhamento de arquivos já cadastrados em documentos no ArqGED:

1. <mark style="color:blue;">**POST**</mark>**&#x20;- Gerar link de compartilhamento**
   * Permite compartilhar arquivos de um documento já existente.
   * Obrigatório: ID do documento e ID do cliente (no cabeçalho da requisição).
   * Opcional: ID de imagem específica e prazo de compartilhamento.
   * Se não for informado o ID da imagem, todos os arquivos do documento serão compartilhados.
   * O retorno inclui ID da imagem, descrição, nome do arquivo e link de compartilhamento.
2. <mark style="color:green;">**GET**</mark>**&#x20;- Consultar links de compartilhamento**
   * Retorna todos os links de compartilhamento de arquivos associados a um documento.
   * Obrigatório: ID do documento e ID do cliente (no cabeçalho).
   * Não há opção de consultar apenas um arquivo específico – a consulta sempre retorna todos os arquivos compartilhados do documento.
3. <mark style="color:red;">**DEL**</mark>**&#x20;- Deletar link de compartilhamento**
   * Permite remover (de forma lógica) o compartilhamento de arquivos.
   * Obrigatório: ID do documento e ID do cliente (no cabeçalho).
   * Opcional: ID da imagem.
   * Caso não seja informado o ID da imagem, todos os compartilhamentos do documento serão removidos.
   * A exclusão não é física: é registrada apenas uma data de expiração para o compartilhamento.

**⚙️ Padrões gerais da API**

* Todas as requisições exigem Subscription Key e token de autorização.
* IDs de documentos, clientes e imagens podem ser obtidos pelos serviços já existentes de busca na API.

</details>

**Integração ArqSign - Maio/2025**

<details>

<summary>21/05 - ArqGED - Integração ArqSIGN</summary>

**Integração com o ArqSIGN**

A integração do ArqFLOW com a ArqSIGN permitirá ao cliente ativar fluxos com assinaturas de documentos via plataforma ArqSIGN.

**Pré-requisitos**

* Serviço “ArqSIGN Plataforma” vigente no contrato do cliente.
* Conta ativa e com assinatura de plano vigente na plataforma ArqSIGN.
* Formulários

**Configurações necessárias**

Inclui o serviço “ArqSIGN Plataforma” no contrato do cliente;

**Cadastrar o desenho do fluxo:**

* Associar o serviço ArqSIGN Plataforma” que consta no contrato do Cliente;
* Configurar os processos de assinatura que irão ocorrer no fluxo;
* Incluir no fluxograma a etapa que cada processo de assinatura ocorrerá.

**Contrato > Serviço**

Inclusão do serviço

Ao selecionar o serviço “ArqSIGN Plataforma”, o sistema exibe os campos para informar os dados da conta ArqSIGN.

* Id Conta ArqSIGN
* Ícone “Validar Conta”
* Nome da Conta ArqSIGN
* Ícone “Informações da Conta”
* GRID para cadastro dos subserviços que serão: Envios, WhatsApp e SMS

[**Workflow > Desenho do Fluxo > ArqSign**](../workflow/desenho-do-fluxo/arqsign.md)

</details>
