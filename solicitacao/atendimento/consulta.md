# 🔹 Consulta

{% embed url="https://app.heygen.com/share/2df059b574ac4a2daabfe1b7f94c564b" %}

Nesta tela são exibidas as solicitações do cliente feitas pelo menu Solicitações > Consulta. Toda a reserva transformada em **Pedido**, fica disponível para atendimento neste local, seja para atendimento realizado pela Unidade Arquivar (Guarda Terceirizada) ou pelo CEDOC do cliente (Guarda Interna).

<figure><img src="../../.gitbook/assets/image (101).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">O painel de atendimento é único e exibe todos os tipos de pedidos realizados no ArqGED:</mark>

* <mark style="color:blue;">Documento original</mark>
* <mark style="color:blue;">Documento digitalizado</mark>
* <mark style="color:blue;">Documento cópia</mark>
* <mark style="color:blue;">Caixa</mark>
* <mark style="color:blue;">Subcaixa</mark>
{% endhint %}

Os campos exibidos no cabeçalho da página são campos disponíveis para “pesquisa” de pedidos.

<figure><img src="../../.gitbook/assets/image (102).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Prioridade:** Exibe para seleção as opções de atendimento disponíveis, geralmente são utilizadas as opções de consulta "normal e urgente".

**Caixa ou Subcaixa:** Campo disponível para inserir o número da caixa ou subcaixa que deseja consultar o pedido.

**Código Documento:** Campo disponível para consultar os pedidos por código do registro.

**Código Consulta:** Permite a localização do pedido pelo número gerado no atendimento da solicitação.

**Tipo de Guarda:** Exibe as opções de guarda sendo elas guarda terceirizada ou guarda interna. Por padrão este campo já aparece preenchido conforme o tipo de usuário logado.

**Empresa:** Quando o usuário logado for de Unidade, será apresentada a lista de clientes de guarda terceirizada.

**Data Início / Data Fim:** Permite a busca de todas as solicitações abertas em determinado período.

**Pesquisar:** Ao clicar neste botão, é realizada a busca dos pedidos conforme dados informados para busca.

<figure><img src="../../.gitbook/assets/image (103).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Editar:** Permite a edição do pedido, selecione o pedido e clique em editar.

**Visualizar:** Permite a visualização do pedido, selecione o pedido e clique em visualizar.

**Distribuir:** O ícone é habilitado na tela de atendimento a consulta sempre que +1 pedido com status “Em Triagem” estiver selecionado no GRID.

Ao pressionar este ícone a aplicação abre uma modal com os campos “Atendente Responsável” e “Destino”.

<figure><img src="../../.gitbook/assets/image (104).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Desta forma o Gerente do atendimento pode realizar a definição do atendente responsável e do destino das solicitações selecionadas em lote.

Não é obrigatório informar os dois campos, ele pode informar somente um campo, desta forma, se for selecionado novamente um universo, e neste pelo menos 1 pedido já tiver a informação de “Atendente Responsável”, estará habilitado somente o campo “Destino” e vice e versa.

<figure><img src="../../.gitbook/assets/image (105).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Exportar:** Permite gerar um arquivo .CSV considerando:

* Informações do Pedido
* Informações dos Itens
* Informações dos Atendimento

O relatório de “Informações dos Atendimentos” é muito utilizado para validação do faturamento, pois, nele são consideradas as informações utilizadas durante o processo.

<figure><img src="../../.gitbook/assets/image (106).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Coluna Tipo:** Exibe o ícone que corresponde ao tipo de volume solicitado.

<figure><img src="../../.gitbook/assets/image (107).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">**Caixa Temporária:**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Somente a unidade consegue fazer este tipo de pedido. Ele deve ser usado quando a caixa ainda não foi indexada e o setor de atendimento precisa procurar um documento dentro desta caixa para enviar ao Cliente. Desta forma nesta consulta se seleciona a caixa, é realizada a busca pelo documento que é enviado  para o cliente. Feito desta forma é gerada uma cobrança de consulta de documento e a caixa não muda o status para "Enviado ao Cliente".</mark>
{% endhint %}

**Coluna Pedido:** Exibe o número de pedido gerado no momento do envio da solicitação de consulta.

**Coluna Cliente:** Exibe o nome do cliente de cada um dos pedidos.

**Coluna Solicitante:** Exibe o nome do usuário que realizou a solicitação no sistema.

**Coluna Atendente:** Exibe o nome do colaborador responsável pelo atendimento da solicitação.

**Coluna Data Envio:** Exibe a data/hora em que o pedido foi efetivado no sistema pelo solicitante.

**Coluna Ordem:** Por padrão o campo “Ordem” sempre vem com o número “10”, e o usuário terá a possibilidade de mudar a ordem do pedido, diminuindo este número e então este pedido ficará na frente dos demais independente do seu SLA. Seria uma forma do Gerente poder priorizar um pedido por questões críticas.

Por padrão, os pedidos são ordenados com a seguinte regra:

1. Ordenados pelo campo “Ordem”
2. Ordenados pelo “Status”
3. Ordenados pelo “SLA” (o mais antigo primeiro)

**Coluna Data SLA:** Exibe a data/hora ou período limite para conclusão do atendimento da solicitação.

**Coluna Data Previsão:** Exibe a data prevista para fechamento do atendimento no sistema.

**Coluna Data Fechado:** Exibe a data de fechamento (conclusão do atendimento) do pedido no sistema.

**Coluna Status:** Exibe em qual fase do fluxo de consulta o pedido está no momento.

**Coluna Destino:** Exibe o destino do item solicitado após busca no local de acondicionamento.

Além dos filtros disponíveis no cabeçalho da tela, existe a possibilidade de aplicação de filtro nas colunas.

<figure><img src="../../.gitbook/assets/image (108).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Ao utilizar o filtro das colunas do Painel de Atendimento, fique atento aos comandos disponíveis para busca:

<figure><img src="../../.gitbook/assets/image (109).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

O ideal, quando o usuário não tiver certeza de como foi escrito o texto que busca, é informar que o filtro deverá considerar tudo que “**Contém**” o texto e informar no filtro parte da informação que deseja buscar.

<figure><img src="../../.gitbook/assets/image (110).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">O usuário</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**solicitante**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">poderá acessar o painel de atendimento para</mark> <mark style="color:blue;"></mark><mark style="color:blue;">**visualizar**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">o andamento da sua solicitação, consultar seu pedido ou exportar dados do pedido em .CSV, porém, não é permitido ao solicitante nenhuma interação com o atendimento da demanda. Apenas o atendente da Unidade Arquivar ou do CEDOC do cliente, poderá prosseguir com o atendimento do pedido no sistema. Para o usuário solicitante não é habilitada a opção de "Editar" o pedido.</mark>
{% endhint %}

***

## Atendimento de um Pedido de Documento <a href="#atendimento-de-um-pedido-de-documento" id="atendimento-de-um-pedido-de-documento"></a>

{% embed url="https://app.supademo.com/demo/cm8hgis7l05c77q3vpw7jf1s0" %}
Clique na legenda e siga o passo a passo.
{% endembed %}

No Painel de Atendimento, selecione o pedido que será trabalhado e clique em editar.

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F1023047207-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FtM1xGMYoU6wC7tnUUXEo%252Fuploads%252FMlckoWR6ig8PZOpiJDMw%252Fimage.png%3Falt%3Dmedia%26token%3D345bfbf0-6ffd-40db-851d-ad6fa46e8df4&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=bd8c24e0&#x26;sv=1" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

A tela de atendimento é dividida em duas abas:

### Aba Dados Gerais

A aba Dados Gerais exibe vários campos inativos para preenchimento, trata-se de informações que foram inseridas ao longo do processo de reserva e abertura do pedido no sistema.

{% hint style="info" %}
<mark style="color:blue;">Tanto para o pedido de documento quanto para o pedido de caixa/subcaixa, a aba “Dados Gerais” apresenta a mesma necessidade de preenchimento para sequência no atendimento do pedido no sistema.</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/image (12) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Quando no fluxo de atendimento do cliente tiver definida a etapa de “**Aprovação**”, o pedido só poderá entrar em atendimento após o responsável imediato no cliente efetuar a aprovação da solicitação, ou seja, quando ele aprovar o pedido.

Essa medida é geralmente utilizada para evitar o **acesso indevido**, de pessoas não autorizadas à determinado acervo.

{% hint style="danger" %}
<mark style="color:red;">A aprovação considera sempre o volume total (documento ou caixa/subcaixa) solicitado no pedido, então se um pedido possui 10 documentos a aprovação autoriza o atendimento dos 10 documentos. Caso o responsável pela aprovação identifique no pedido algum item que não deve ser autorizado, todo o pedido deve ser cancelado e o processo realizado novamente pelo solicitante, desconsiderando o item não autorizado pelo Gestor.</mark>
{% endhint %}

Para “Aprovar” ou “Cancelar” o pedido, o responsável deverá acessar a tela Solicitação > Atendimento > Consulta, identificar e abrir o pedido, clicar em “Salvar” e depois em “Processar” para aprovar ou no caso de cancelamento, clicar em "Salvar" e depois em “Cancelar Pedido”.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Aprovado o pedido, o status é alterado e uma nova ação é registrada.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Feita a aprovação, o status do pedido é alterado para "Triagem" e o pedido fica disponível para andamento do atendimento, além de gerar uma nova ação para o atendimento.

{% hint style="info" %}
<mark style="color:blue;">A data e Hora registrada no campo “Ação”, sinaliza a hora que a ação foi gerada no ArqGED e não a hora de efetivação, por exemplo, na imagem a “Aprovação” foi gerada em 09/08/2024, ou seja, o pedido ficou aguardando aprovação a partir desta data. Em 12/11/2024 o pedido foi aprovado e gerada a ação de “Triagem”, ou seja, o pedido teve sua aprovação efetivada no sistema em 12/11/2024.</mark>
{% endhint %}

Retornando ao atendimento do pedido, agora aprovado, o atendente deverá iniciar com o preenchimento dos campos:

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Ordem:** Por padrão o campo é exibido preenchido com a informação "10", neste momento o atendente poderá reduzir esta numeração, o que altera a prioridade de atendimento deste pedido no painel de atendimento.

**Status:** Exibe o status do pedido em questão.

**Destino:** Exibe a lista de possibilidades de envio do pedido ao concluir a fase de triagem.

**Atendente:** Selecione neste campo o nome do atendente que irá seguir com o atendimento do pedido no sistema. Identificar o atendente responsável pelo pedido, impede que mais de uma pessoa fique dedicada ao mesmo trabalho/atendimento.

Preenchidos todos os campos, clique "salvar" para prosseguir. Após salvar, os botões “Cancelar Pedido” e “Guia” são habilitados e para utilização.

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Cancelar Pedido:** O identificar alguma inconsistência, o atendente pode realizar o cancelamento do pedido. Ao optar por desistir do pedido, será apresentada uma mensagem de confirmação da ação. Ao confirmar o pedido é cancelado e o documento volta a ficar disponível para nova reserva.

**Guia:** Ao clicar neste botão, é aberta a Guia de Busca de Documentos. Esta guia pode ser impressa e entregue ao auxiliar de arquivo para que realize a busca do volume no Arquivo.

#### **Guia de Busca de Documentos**

<figure><img src="../../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

No cabeçalho da Guia é exibido:

* **Pedido:** Exibe o número do pedido de caixa criado no ArqGED.
* **Dados do solicitante:**
  * Nome do cliente
  * Data/Hora de abertura do pedido
  * Nome do solicitante no ArqGED
  * Telefone do solicitante

<figure><img src="../../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Abaixo é exibida:

* Listagem dos documentos solicitados no pedido com a associação da caixa de guarda onde estão alocados
* Endereço das caixas
* Forma de entrega definida pelo solicitante
* Destino, ou seja, para onde o documento deve ser encaminhado para andamento do atendimento
* Local para o auxiliar de arquivo sinalizar se a caixa foi localizada no arquivo

<figure><img src="../../.gitbook/assets/image (8) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Por fim, são exibidos campos que identificam os atores atuantes no atendimento:

* Atendente Responsável
* Auxiliar de Arquivo responsável pela consulta
* Auxiliar de Arquivo responsável pela Devolução
* Data/Hora da Impressão da guia

<figure><img src="../../.gitbook/assets/image (9) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">Quando a Unidade possui configuração definida para</mark> [<mark style="color:blue;">Grupo de Endereços</mark>](../configuracao/grupo-de-endereco.md)<mark style="color:blue;">, é gerada uma guia de busca por grupo. Isso é feito para que o auxiliar de arquivo responsável pela busca dos volumes  no arquivo tenha maior facilidade e produtividade na separação do acervo.</mark>
{% endhint %}

Concluído o processo de busca no arquivo, o atendente precisa informar para o sistema que a etapa foi realizada para prosseguir com o atendimento.

Para seguir com o atendimento, clique “Processar”.

<figure><img src="../../.gitbook/assets/image (10) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Ao processar o atendimento, um novo status é definido e uma nova ação é listada na tela.

<figure><img src="../../.gitbook/assets/image (11) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

***

### Aba Detalhes

Nesta aba, são listados todos os documentos do pedido. É nesta tela que são adicionadas as informações específicas do atendimento.

**Detalhes de um Pedido de Documentos**

<figure><img src="../../.gitbook/assets/image (12) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Grupo:** Quando a Unidade possui configuração definida para [Grupo de Endereços](../configuracao/grupo-de-endereco.md), este campo é apresentado na tela e é considerado para organização do pedido. Isso é feito para que o auxiliar de arquivo responsável pela busca dos volumes  no arquivo tenha maior facilidade e produtividade na separação do acervo.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Coluna Seleção:** Exibe um local para seleção do atendimento.

**Coluna Doc:** Ao clicar no ícone o registro é apresentado na tela e é possível navegar entre as abas do registro existente no ArqGED.

<figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Coluna Atend:** Clicando no ícone é possível acessar as particularidades do atendimento, onde de fato são adicionadas as informações para seguir com o processo.

**Coluna Info:** Clicando no ícone, é exibida a mensagem inserida na tela de reservas, quando houver.

**Coluna Documento:** Exibe um resumo dos dados metadados do documento/registro solicitado.

**Colunas Buscas:** Exibe a quantidade de buscas realizadas no arquivo para localização do documento solicitado. Essa informação deve ser preenchida pelo atendente no momento de fechamento do pedido no ArqGED.

**Coluna Cópias:** Exibe a quantidade de cópias geradas para o documento solicitado. Essa informação deve ser preenchida pelo atendente no momento de fechamento do pedido no ArqGED.

**Coluna Img.:** Exibe a quantidade de imagens geradas para o documento solicitado. Essa informação deve ser preenchida pelo atendente no momento de fechamento do pedido no ArqGED.

**Coluna Localizado:** Exibe se o documento foi encontrado no seu local de guarda pelo auxiliar de arquivo. Essa informação deve ser preenchida pelo atendente no momento de fechamento do pedido no ArqGED.

**Colunas Carregado / Entregue / Auxiliar:** São exibidas sem informação, pois não são utilizadas atualmente.

Para o preenchimento destes dados, é necessário acessar o ícone de "Atendimento" para cada um dos documentos solicitados. Clique no ícone para prosseguir:

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Uma nova tela será exibida na tela para preenchimento:

<figure><img src="../../.gitbook/assets/image (15).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Considerar / Desconsiderar:** Quando selecionado “Considerar”, o sistema permite o andamento do atendimento com a inclusão dos dados e fechamento do pedido, inclusive obrigando o preenchimento do campo "Descrição do Item". Quando selecionado “Desconsiderar”, o pedido fica “Pendente” aguardando até que o preenchimento dos dados do atendimento seja realizado, isso impedirá que outro atendente finalize o pedido de forma indevida.

**Descrição do Item:** Este campo possibilita a inclusão de informações relevantes ao documento, por exemplo: Dossiê de Admissão funcionário X. Trata-se de um campo de preenchimento obrigatório para prosseguimento do atendimento.

**Localizado / Não Localizado:** Exibe a informação de sucesso na localização do documento no arquivo. Selecione conforme realidade do seu pedido.

**Original / Não Original:** Exibe a forma como o documento está sendo disponibilizado ao cliente.

**Total / Parcial:** Quando selecionado “Total”, indica que o registro ficará totalmente em consulta e indisponível para novas solicitações até que seja feita a devolução do registro que no caso é o documento. Quando selecionado "Parcial", indica que o registro representa um lote de documento, como por exemplo: NF de 1 a 1.000. Então o cliente solicita somente NF número 10, então o atendente enviará somente a nota 10 e o registro ficará disponível para novas consultas. Neste caso, o registro fica com status em consulta parcial (que significa que uma parte do lote está disponível, e por isso o cliente consegue fazer solicitações selecionando o mesmo registro antes da devolução da NF 10.)

**Simples / Complexa:** Exibe a classificação do pedido, se deve ser tratado como uma consulta simples ou complexa (definição realizada no contrato de prestação de serviços).

**Código:** Este campo deve ser preenchido considerando o código de consulta. O código de consulta é controlado por unidade e geralmente é fornecido pela Master que disponibiliza uma planilha para acompanhamento da unidade. Os códigos são gerados considerando o padrão EAN-8, que é reconhecido pelo ArqGED que verifica se o código informado já foi utilizado para aquela unidade.

{% hint style="success" %}
<mark style="color:green;">A Master orienta que de posse da planilha de códigos, cada Unidade realize a impressão do seu sequencial com códigos de barras para que no momento do atendimento da consulta a etiqueta seja colada no verso do documento para identificar a movimentação, facilitar o processo de devolução e torná-lo mais seguro. Neste cenário é muito utilizada a impressão de etiquetas em rolo. Caso a Unidade opte por não realizar a impressão de seus códigos, o atendente deve anotar manualmente no verso do documento o código utilizado no atendimento da consulta.</mark>&#x20;
{% endhint %}

**Buscas:** Registre neste campo a quantidade de buscas realizadas para localização do documento em questão.

**Cópias:** Registre neste campo a quantidade de cópias geradas para o documento solicitado, quando for o caso.

**Digital:** Registre neste campo a quantidade de imagens geradas com a digitalização do documento para atendimento do pedido.

**Observação:** Utilize este campo para registrar informações relevantes ao atendimento do pedido.

**Arraste os arquivos para esta área...:** Quando o atendimento for realizado através da digitalização do documento, adicione o arquivo neste local.

O documento uma vez solicitado em formato digital e adicionado no atendimento do pedido, terá a imagem armazenada no ArqGed como “anexo do documento”. Em uma próxima necessidade de consultar/visualizar o documento, o solicitante não precisa abrir novo pedido, basta localizar o arquivo no ArqGED e visualizar novamente a imagem.

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Finalizado o preenchimento das informações de atendimento do pedido, clique “Incluir” para prosseguir.

<figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Neste momento os dados do atendimento são inseridos em “Itens Salvos”.

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="danger" %}
<mark style="color:red;">Ao realizar o fechamento de um atendimento, fique muito atento no momento de lançar as quantidades, pois, é deste lançamento que é feita a apuração das quantidades executadas para cobrança/faturamento.</mark>
{% endhint %}

Retornando para a tela inicial, são apresentados os dados preenchidos no atendimento.

Selecione o próximo documento e repita o processo até que todos os documentos do pedido tenham o lançamento dos dados de atendimento realizados.

<figure><img src="../../.gitbook/assets/image (19).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Após o lançamento dos dados de atendimento, é possível emitir o “Protocolo de Consulta de Documentos” para envio ao cliente, caso o pedido seja de envio do acervo.

<figure><img src="../../.gitbook/assets/image (21).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

No protocolo é identificado:

* O número do pedido
* Os dados do cliente solicitante
* Controle de Sinistro
* A relação dos itens do pedido
* Os dados dos responsáveis pelo recebimento (Solicitante)
* Os dados dos responsáveis pela entrega (CEDOC)

Emitido o protocolo, retorne para a tela do atendimento e clique “Processar”, para atualização do pedido que vai para “Fechamento”.

<figure><img src="../../.gitbook/assets/image (22).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Ao clicar novamente em “Processar”, o pedido é fechado no sistema e o documento é encaminhado ao cliente.

<figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">Sempre que o pedido é encerrado no ArqGED, o solicitante é notificado por e-mail quanto ao encerramento do seu pedido.</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/image (24).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

***

## Atendimento de um Pedido de Caixa ou Subcaixa

{% embed url="https://app.supademo.com/demo/cm8hob2iy01c22pzhn3opn9c2" %}
Clique na legenda e siga o passo a passo.
{% endembed %}

No Painel de Atendimento, selecione o pedido que será trabalhado e clique em editar.

<figure><img src="../../.gitbook/assets/image (111).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

A tela de atendimento é dividida em duas abas:

### Aba Dados Gerais

A aba Dados Gerais exibe vários campos inativos para preenchimento, trata-se de informações que foram inseridas ao longo do processo de reserva e abertura do pedido no sistema.

{% hint style="info" %}
<mark style="color:blue;">Tanto para o pedido de documento quanto para o pedido de caixa/subcaixa, a aba “Dados Gerais” apresenta a mesma necessidade de preenchimento para sequência no atendimento do pedido no sistema.</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/image (112).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Quando no fluxo de atendimento do cliente tiver definida a etapa de “**Aprovação**”, o pedido só poderá entrar em atendimento após o responsável imediato no cliente efetuar a aprovação da solicitação, ou seja, quando ele aprovar o pedido.

Essa medida é geralmente utilizada para evitar o **acesso indevido**, de pessoas não autorizadas à determinado acervo.

{% hint style="danger" %}
<mark style="color:red;">A aprovação considera sempre o volume total (documento ou caixa/subcaixa) solicitado no pedido, então se um pedido possui 10 caixas a aprovação autoriza o atendimento das 10 caixas. Caso o responsável pela aprovação identifique no pedido algum item que não deve ser autorizado, todo o pedido deve ser cancelado e o processo realizado novamente pelo solicitante, desconsiderando o item não autorizado pelo Gestor.</mark>
{% endhint %}

Para “Aprovar” ou “Cancelar” o pedido, o responsável deverá acessar a tela Solicitação > Atendimento > Consulta, identificar e abrir o pedido, clicar em “Salvar” e depois em “Processar” para aprovar ou no caso de cancelamento, clicar em "Salvar" e depois em “Cancelar Pedido”.

<figure><img src="../../.gitbook/assets/image (113).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Aprovado o pedido, o status é alterado e uma nova ação é registrada.

<figure><img src="../../.gitbook/assets/image (114).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Feita a aprovação, o status do pedido é alterado para "Triagem" e o pedido fica disponível para andamento do atendimento, além de gerar uma nova ação para o atendimento.

{% hint style="info" %}
<mark style="color:blue;">A data e Hora registrada no campo “Ação”, sinaliza a hora que a ação foi gerada no ArqGED e não a hora de efetivação, por exemplo, na imagem a “Aprovação” foi gerada em 09/08/2024, ou seja, o pedido ficou aguardando aprovação a partir desta data. Em 12/11/2024 o pedido foi aprovado e gerada a ação de “Triagem”, ou seja, o pedido teve sua aprovação efetivada no sistema em 12/11/2024.</mark>
{% endhint %}

Retornando ao atendimento do pedido, agora aprovado, o atendente deverá iniciar com o preenchimento dos campos:

<figure><img src="../../.gitbook/assets/image (115).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Ordem:** Por padrão o campo é exibido preenchido com a informação "10", neste momento o atendente poderá reduzir esta numeração, o que altera a prioridade de atendimento deste pedido no painel de atendimento.

**Status:** Exibe o status do pedido em questão.

**Destino:** Exibe a lista de possibilidades de envio do pedido ao concluir a fase de triagem.

**Atendente:** Selecione neste campo o nome do atendente que irá seguir com o atendimento do pedido no sistema. Identificar o atendente responsável pelo pedido, impede que mais de uma pessoa fique dedicada ao mesmo trabalho/atendimento.

Preenchidos todos os campos, clique salvar para prosseguir. Após salvar, os botões “Cancelar Pedido” e “Guia” são habilitados e para utilização.

<figure><img src="../../.gitbook/assets/image (116).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Cancelar Pedido:** O identificar alguma inconsistência, o atendente pode realizar o cancelamento do pedido. Ao optar por desistir do pedido, será apresentada uma mensagem de confirmação da ação. Ao confirmar o pedido é cancelado e o documento volta a ficar disponível para nova reserva.

**Guia:** Ao clicar neste botão, é aberta a Guia de Busca de Documentos. Esta guia pode ser impressa e entregue ao auxiliar de arquivo para que realize a busca do volume no Arquivo.

**Guia de Busca de Caixas e Subcaixas**

Em ambos os casos a guia possui a mesma estrutura, a diferença delas está no título e na informação do volume: caixa ou subcaixa.

<figure><img src="../../.gitbook/assets/image (117).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

No cabeçalho é exibido:

* Pedido: Exibe o número do pedido de caixa ou subcaixa criado no ArqGED.

Dados do solicitante:

* Nome do cliente
* Data/Hora de abertura do pedido
* Nome do solicitante no ArqGED
* Telefone do solicitante

<figure><img src="../../.gitbook/assets/image (118).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Logo abaixo é exibida:

* Listagem das caixas e/ou subcaixas solicitadas no pedido
* Endereço das caixas e/ou subcaixas
* Local para o auxiliar de arquivo (responsável CEDOC) sinalizar se a caixa ou subcaixa foi localizada no arquivo

<figure><img src="../../.gitbook/assets/image (119).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Por fim, são exibidos campos que identificam os atores atuantes no atendimento:

* Atendente Responsável (responsável CEDOC)
* Auxiliar de Arquivo responsável pela consulta (responsável CEDOC)
* Auxiliar de Arquivo responsável pela Devolução (responsável CEDOC)
* Data/Hora da Impressão da guia

<figure><img src="../../.gitbook/assets/image (121).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">Quando a Unidade possui configuração definida para</mark> [<mark style="color:blue;">Grupo de Endereços</mark>](../configuracao/grupo-de-endereco.md)<mark style="color:blue;">, é gerada uma guia de busca por grupo. Isso é feito para que o auxiliar de arquivo responsável pela busca dos volumes  no arquivo tenha maior facilidade e produtividade na separação do acervo.</mark>
{% endhint %}

Concluído o processo de busca no arquivo, o atendente precisa informar para o sistema que a etapa foi realizada para prosseguir com o atendimento.

Para seguir com o atendimento, clique “Processar”.

<figure><img src="../../.gitbook/assets/image (122).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Ao processar o atendimento, um novo status é definido e uma nova ação é listada na tela.

<figure><img src="../../.gitbook/assets/image (123).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Aba Detalhes

Nesta aba, são listados todas as caixas ou subcaixas do pedido. É nesta tela que são adicionadas as informações específicas do atendimento.

#### Detalhes de um Pedido de Caixa

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Grupo:** Quando a Unidade possui configuração definida para Grupo de Endereços, este campo é apresentado na tela e é considerado para organização do pedido. Isso é feito para que o auxiliar de arquivo responsável pela busca dos volumes no arquivo tenha maior facilidade e produtividade na separação do acervo.

<figure><img src="../../.gitbook/assets/image (125).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Coluna Seleção:** Exibe um local para seleção do atendimento.

**Coluna Atend:** Clicando no ícone é possível acessar as particularidades do atendimento, onde de fato são adicionadas as informações para seguir com o processo.

**Coluna Caixa:** Exibe o código da caixa solicitada.

**Coluna Endereço:** Exibe o local de alocação da caixa no arquivo.

**Coluna Itens:** Exibe a quantidade de registros existentes no sistema para a caixa solicitada.

**Coluna Localizado:** Exibe se a caixa foi encontrado no seu local de guarda pelo auxiliar de arquivo. Essa informação deve ser preenchida pelo atendente no momento de fechamento do pedido no ArqGED.

**Colunas Carregado / Entregue / Auxiliar:** São exibidas sem informação, pois não são utilizadas atualmente.

#### **Detalhes de um pedido de Subcaixa**

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Coluna Seleção:** Exibe um local para seleção do atendimento.

**Coluna Atend:** Clicando no ícone é possível acessar as particularidades do atendimento, onde de fato são adicionadas as informações para seguir com o processo.

**Coluna Subcaixa:** Exibe o código da Subcaixa solicitada e a referência da sua caixa de origem.

**Coluna Endereço:** Exibe o local de alocação da caixa de origem no arquivo.

**Coluna Itens:** Exibe a quantidade de registros existentes no sistema para a caixa solicitada.

**Coluna Localizado:** Exibe se a caixa foi encontrado no seu local de guarda pelo auxiliar de arquivo. Essa informação deve ser preenchida pelo atendente no momento de fechamento do pedido no ArqGED.

**Colunas Carregado / Entregue / Auxiliar:** São exibidas sem informação, pois não são utilizadas atualmente.

Para o preenchimento destes dados, é necessário acessar o ícone de "Atendimento" para cada uma das caixas ou subcaixas solicitadas. Clique no ícone para prosseguir:

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Uma nova tela será aberta para preenchimento dos dados de atendimento.

Por padrão a tela é apresentada com uma mensagem de alerta quanto ao status do pedido. Se o pedido já estiver com o status correto, clique em editar para prosseguir, caso contrário retorne para a aba dados gerais e conclua o preenchimento necessário para alteração do status.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Localizado / Não Localizado:** Exibe a informação de sucesso na localização da caixa no arquivo. Selecione conforme realidade do seu pedido.

**Descrição do Item:** Este campo possibilita a inclusão de informações relevantes ao pedido de caixa/Subcaixa, caso possua, informe no local indicado e clique em salvar.

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Após o lançamento da informação de localização da caixa/subcaixa, é possível emitir o “Protocolo de Consulta de Caixas” ou “Protocolo de Consulta de Subcaixa” para envio ao solicitante, caso o pedido seja de envio do acervo para a área solicitante.

<figure><img src="../../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Tanto no protocolo de consulta de Caixa quanto no de consulta de subcaixa, são exibidas as informações:

* O número do pedido
* Os dados do cliente solicitante
* Controle de Sinistro
* A relação dos itens do pedido (caixas ou subcaixas)
* Os dados dos responsáveis pelo recebimento (cliente)
* Os dados dos responsáveis pela entrega (Unidade Arquivar).

Emitido o protocolo, retorne para a tela do atendimento e clique “Processar”, para atualização do pedido que vai para “Fechamento”.

<figure><img src="../../.gitbook/assets/image (6) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Ao clicar novamente em “Processar”, o pedido é fechado no sistema e a caixa/subcaixa é encaminhada ao cliente.

<figure><img src="../../.gitbook/assets/image (7) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Realizado o processamento do pedido, a lista de ações é atualizada.

No Painel de Atendimento, as informações são atualizadas podendo ser visualizadas pelo solicitante.

<figure><img src="../../.gitbook/assets/image (10) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">Sempre que o pedido é encerrado no ArqGED, o solicitante é notificado por e-mail quanto ao encerramento do seu pedido.</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/image (11) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>
