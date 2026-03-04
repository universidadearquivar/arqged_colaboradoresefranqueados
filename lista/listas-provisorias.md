# 🟩 Listas Provisórias

Neste Submenu deve ser feita a configuração da Lista Provisória, conforme nó de árvore correspondente.

Na tela inicial do submenu, temos:

<figure><img src="../.gitbook/assets/image (368).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Cliente:** É exibida uma lista com todos os clientes da Unidade para seleção.

**Adicionar:** Permite a inclusão da configuração de uma nova lista.

**Editar:** Após selecionar uma lista na tela, ao clicar no ícone é possível editar os dados de uma lista já configurada.

**Visualizar:** Após selecionar uma lista na tela, ao  clicar neste ícone, é possível visualizar todas as informações inseridas no cadastro de uma lista provisória.

**Excluir:** Após selecionar a lista, ao clicar no ícone a lista é excluída.

**Atualizar:** Inserida uma nova lista ou excluída, clique no ícone para atualização do status da lista criada.

<figure><img src="../.gitbook/assets/image (369).png" alt=""><figcaption><p>Clique ne imagem para ampliar.</p></figcaption></figure>

**Coluna Nome da Lista:** Exibe o nome definido para a lista no momento do cadastro.

**Coluna Árvore Documental:** Exibe a Árvore selecionada uso da lista no momento do cadastro.

**Coluna Data de Expiração:** Exibe a data definida para limite de uso da lista.

**Coluna Itens Restantes:** Exibe a contagem dos itens existentes na lista ainda não utilizados na indexação, além de permitir pelo ícone de download a exportação desses itens.

**Coluna Status:** Exibe o status do cadastro da lista no ArqGED.

## Configurando uma Lista Provisória

Acesse o Menu Lista > Listas Provisórias > Adicionar.

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Realize o preenchimento dos dados conforme solicitado na tela:

**Nome da Lista:** Informe um nome para a lista, importante fazer referência ao processo em que estará vinculada, por exemplo: Indexação de Nota Fiscal de Entrada. Este campo será validado e caso o nome esteja repetido, o usuário não conseguirá seguir com o cadastro.

**Data de Expiração:** Informe a data limite para uso da lista. Por padrão a lista vence em três meses,  considerando a data de cadastro como base. Quando inserida uma data com prazo superior aos três meses, ao clicar em salvar, será exibida na tela uma mensagem de erro informando a data limite de expiração para a lista.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">É importante que o</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**responsável pelo projeto**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">se organize para</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**controlar a expiração**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">da lista junto dos prazos de indexação. Caberá ao responsável</mark> <mark style="color:orange;"></mark><mark style="color:orange;">**renovar o prazo**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">de expiração no sistema, o que pode ser realizado quantas vezes forem necessárias.</mark>

<mark style="color:orange;">Um ponto importante sobre a validade da lista é  que  sempre que ocorrer uma importação de novos itens nesta lista, o prazo é postergado automaticamente pelo sistema.</mark>
{% endhint %}

**Universo de trabalho:** Selecione o universo de trabalho onde a lista será utilizada.

**Árvore Organizacional:** Defina em qual nível de árvore os campos customizados que utilizarão a lista estarão disponíveis. Neste caso, não é obrigatório que os campos customizados estejam associados ao último nível da árvore.

**Carregar dados da lista provisória:** Arraste ou selecione o arquivo com os dados, considerando as particularidades:

* O arquivo precisa ser da extensão CSV, com separador ; (ponto e vírgula)&#x20;
* Na primeira linha do arquivo deve conte o IdCampoCustomizado
* Cada coluna deve conter os dados de um único campo customizado
* O arquivo pode ter no máximo 15 colunas  - o total de colunas já existentes na tabela e as novas colunas do arquivo, não devem ultrapassar 15 colunas
* O arquivo deve ter no máximo 1 milhão de linhas - o total de linha de dados no arquivo somados ao total de dados já existentes na tabela, não deve ultrapassar 1 milhão de linhas de dados

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

Ao carregar o arquivo, são exibidos na tela na coluna "Campos da Planilha a combinação:

**Código do campo customizado + o nome + o tipo do campo no sistema.**

**Coluna Chave:** Selecione qual ou quais serão os campos serão utilizados para consultar os demais dados no banco. É permitida a seleção de até dois campos chave por lista. Um campo chave não pode ser um campo "Preview".

**Coluna Preview:** É permitida a seleção de mais de um campo "Preview", quando feito, é habilitado o campo "Ordem" para que seja indicada a ordem de apresentação do campo na indexação.

**Coluna Ordem:** É habilitado para preenchimento conforme uso da coluna anterior "Preview", ela é utilizada para definir a ordem de apresentação dos campos de indexação. É permitido habilitar até três campos como preview.

**Coluna Importação:** Exibe ícones que indicam o sucesso ou não da importação da planilha.

