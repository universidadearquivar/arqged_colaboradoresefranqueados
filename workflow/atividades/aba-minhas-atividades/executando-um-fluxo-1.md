# ➡️ Executando um fluxo - Exibição Listagem

## Visualização Listagem

No modo de exibição 'Listagem', os fluxos sob responsabilidade do usuário logado são exibidos de forma simplificada, em uma lista que destaca as informações mais importantes.

Esse modo de visualização pode ser definido como padrão no [perfil do usuário](../../../administracao/usuarios.md#aba-perfil), garantindo que, ao acessar a aplicação, a tela de Minhas Atividades seja sempre apresentada nessa configuração.

<figure><img src="../../../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Coluna Nº:** Exibe o número/código do fluxo ou número do processo.

**Coluna Processo:** Exibe o nome que é dado ao fluxo na configuração da etapa realizada no momento do desenho do fluxo.

**Coluna Tarefa:** Exibe o nome definido para a tarefa no momento das configurações e desenho do fluxo e ao direcionar o mouse sobre o ícone, é exibida a situação do fluxo (em dia - ícone verde, atrasado - ícone vermelho), o status e a classificação, além das obrigatoriedades.

**Coluna Início Tarefa:** Exibe a data/hora de chegada da tarefa para execução do responsável.

**Coluna Concluir Até:** Exibe a data limite para execução da tarefa, convertendo o prazo configurado para uma data/hora específica de conclusão. Tarefas do tipo ArqSign exibirão o campo vazio, pois não possuem prazo de conclusão e por este motivo serão exibidas sempre no topo da lista.

**Coluna Detalhes:** Exibe os detalhes do fluxo, que são os "Dados Gerais do Processo" , a "Ação da Tarefa Anterior", o nome do responsável anterior, o último comentário, o formulário e os "Dados da Tarefa Atual". Quando houver, serão exibidas também na modal de detalhes as "Instruções para a Tarefa", que são as informações adicionadas no campo "Descrição da Etapa" no momento da configuração da etapa no desenho do fluxo.&#x20;

**Coluna Ações:** Exibe além da opção de "Abrir" o fluxo para tratamento,  a lista de botões  de avanço disponíveis para o processo, como por exemplo: delegar tarefa, voltar para a etapa anterior, cancelar fluxo ou visualizar fluxograma.

#### **Barra de Filtro**

É possível realizar a busca de tarefas utilizando a barra de filtro, que faz a busca de tarefas do usuário utilizando palavras-chave.

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

## Ativar Novo Fluxo

1\. Para ativar um novo fluxo, no menu [Workflow > Atividades > Aba Minhas Atividades](./) clique no botão “Ativar Novo Fluxo”.

2\. Informe o nome da empresa no campo “Cliente”.

3\. No campo “Selecione um Processo”, selecione o fluxo que deseja ativar.

4\. Se houverem observações, informe-as no campo “Observação”. Caso contrário, deixe o campo em branco. As observações inseridas aqui serão exibidas na tela de execução das tarefas.

5\. Selecione se o fluxo terá início imediato (ativar o fluxo no ato) ou se terá o início agendado (com data estabelecida futura).

<figure><img src="../../../.gitbook/assets/minhas_ativ02.png" alt=""><figcaption></figcaption></figure>

6. Clique em “Ativar”. Caso seja um fluxo com início agendado, informe a data e hora para ativação e clique em “Agendar”.

<figure><img src="../../../.gitbook/assets/minhas_ativ03.png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
<mark style="color:red;">**Desenhos de fluxo que possuírem o parâmetro "Bloquear a ativação manual deste fluxo sem um documento associado" selecionado (aba Desenho do Fluxo > Aba Dados Gerais), não poderão ser ativados manualmente pelo botão Ativar Novo Fluxo, da aba Minhas Atividades, porque não poderão ser ativados sem que haja um documento selecionado para associação ao fluxo.**</mark>
{% endhint %}

***

### Executando o Fluxo

Para executar um fluxo, é possível acessá-lo pelo botão **"Abrir Tarefa"**, disponível no botão de "**Detalhes**":

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Ou pelo botão "**Abrir Tarefa"**, disponível na lista de "**Ações"**:

<figure><img src="../../../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Ao abrir o fluxo, será exibida a seguinte tela:

<figure><img src="../../../.gitbook/assets/image (77).png" alt=""><figcaption></figcaption></figure>

1. **Título:** Exibe o nome do Fluxo.
2. **Fechar:** Apenas fecha o fluxo, retornando para a tela inicial com a lista de fluxos pendentes.
3. **Outras ações:** Exibe uma lista de outros caminhos possíveis no fluxo, tais como:

• **Delegar Tarefa:** Permite o envio da Tarefa para outro usuário apenas para conhecimento da demanda ou delegando totalmente.

<figure><img src="../../../.gitbook/assets/image (82).png" alt=""><figcaption></figcaption></figure>

• **Cancelar Fluxo:** Permite cancelar o Processo de Trabalho.

<figure><img src="../../../.gitbook/assets/image (120).png" alt=""><figcaption></figcaption></figure>

• **Visualizar Fluxograma:** Permite que o usuário acesse o Desenho do Processo.

<figure><img src="../../../.gitbook/assets/image (146).png" alt=""><figcaption></figcaption></figure>

4. **Botões de Avanço:** Exibe para o usuário os caminhos disponíveis para tratamento do fluxo.

<figure><img src="../../../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>

5. **Dados Gerais do Processo:** Exibe as informações do processo de trabalho, incluindo Ação da tarefa anterior e responsável.
6. **Dados da Tarefa Atual:** Exibe as informações da etapa atual.
7. **Instrução para tarefa:** Exibe as orientações para execução da tarefa atual, quando se aplica.
8. **Legenda das Cores:** Exibe a classificação de cores para ações, sendo ações obrigatórias (vermelho), ações concluídas (verde) e ações opcionais (azul).

<figure><img src="../../../.gitbook/assets/image (169).png" alt=""><figcaption></figcaption></figure>

9\. **Áreas:** São exibidas as áreas configuradas para o processo no desenho do fluxo, considerando obrigatoriedades e a definição da ordem em que elas devem ser exibidas para o usuário.

{% hint style="info" %}
O nome exibido para a Área, é o nome definido pelo usuário no momento da configuração do campo.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

Ao posicionar o mouse sobre o ícone de "Ação obrigatória pendente", é exibida a lista de pendências que deve ser verificada pelo usuário para aquela área em específico.&#x20;

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

Ao clicar na modal do lado direito da tela, a área é expandida para que o usuário realize as interações necessárias para conclusão das obrigatoriedades.

***
