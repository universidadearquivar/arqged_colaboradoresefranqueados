# 🟩 Regra de Auditoria

Nesta tela, o usuário define regras que possibilitam o controle e a identificação dos documentos ausentes em seu acervo, com base em parâmetros previamente estabelecidos para validação. Essas regras são essenciais para garantir que a documentação esteja completa e em conformidade com as exigências legais ou internas da organização.

Por exemplo, ao admitir um funcionário, é necessário a realização de um exame para emissão do Atestado de Saúde Ocupacional (ASO) - Admissional, logo, é possível criar uma regra no sistema, onde é informado que o documento precisa constar na pasta do funcionário uma única vez dias antes da data de admissão.

Considerando este cenário, o sistema deverá verificar se o ASO consta ou não nos documentos cadastrados para o funcionário em questão e, se não identificado o cadastro desse documento, o sistema deverá apontar sua falta pelo processamento da regra de auditoria.&#x20;

O fluxo deve ser:

{% tabs %}
{% tab title="1. Criação de Regras" %}
O responsável pela gestão cria regras no sistema, definindo qual documento é necessário em determinadas situações. Por exemplo, "O ASO Admissional deve ser registrado uma única vez na pasta do funcionário até 10 dias antes da admissão."
{% endtab %}

{% tab title="2. Verificação Manual ou Automática" %}
Quando um novo funcionário é admitido e seu perfil é atualizado no sistema, baseado na execução automática ou manual da regra de auditoria, o sistema verifica se o ASO Admissional foi registrado na pasta de documentos do colaborador.
{% endtab %}

{% tab title="3. Auditoria e Validação" %}
O sistema, por meio de uma auditoria automatizada, verifica se o documento especificado na regra (neste caso, o ASO) está presente na pasta de documentos do funcionário.
{% endtab %}

{% tab title="4. Alerta Falta de Documento" %}
Caso o ASO não seja encontrado, o sistema gera um alerta, indicando a falta do documento. Esse alerta pode ser enviado para os responsáveis pela gestão de documentos, RH ou outro setor relevante para que a pendência seja corrigida. Um relatório de inconsistência é gerado e disponibilizado para consulta.
{% endtab %}
{% endtabs %}

Este processo visa garantir que os documentos obrigatórios sejam registrados corretamente e dentro dos prazos estabelecidos, evitando falhas ou pendências no cumprimento de exigências legais ou internas da empresa.

{% hint style="warning" %}
<mark style="color:orange;">O processo de auditoria não se limita exclusivamente aos documentos de funcionários, ele é aplicável a todos os tipos documentais que possuem critérios para verificação de sua existência no acervo.</mark>
{% endhint %}

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Cliente:** É apresentado o nome do cliente conforme usuário logado ou conforme selecionado pela Unidade na lista de clientes com o serviço de auditoria ativo em contrato.

**Adicionar:** O ícone é utilizado para adicionar uma nova regra para o cliente selecionado.

**Editar:** Permite a edição de regras já existentes para o cliente, basta selecionar a regra desejada e clicar na opção de editar.

**Visualizar:** Permite ao usuário acessar os parâmetros configurados para a regra, para isso, selecione a regra desejada e clique em visualizar.

**Excluir:** Permite a exclusão de uma regra existente para o cliente. Selecione a regra na tela e clique em excluir.

**Processar:** Permite ao usuário processar a regra de auditoria de forma “manual”, para isso, selecione a regra clique no ícone.

{% hint style="warning" %}
<mark style="color:orange;">Para que o cliente consiga criar uma regra no</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**Menu > Auditoria**</mark><mark style="color:orange;">, é necessário que ele tenha cadastrado em seu contrato vigente o serviço “</mark><mark style="color:orange;">**ArqAudit por Regra**</mark><mark style="color:orange;">”, do contrário ele não poderá criar uma regra de auditoria no sistema.</mark>
{% endhint %}
