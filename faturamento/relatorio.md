# 🟩 Relatório

Neste menu a unidade Arquivar pode gerar os relatórios de faturamento de seus clientes, informando o mês e ano desejados, o intervalo de dias e o cliente.  Esse relatório pode ser gerado em Excel ou em PDF.&#x20;

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/faturamento6.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Sempre que o usuário acessar esta tela, no período fechado ou já faturado para a Unidade ou Unidade cliente, é exibido o link de acesso ao último relatório gerado em PDF ou Excel.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### Faturamento período "Em aberto"

Quando não houver relatório solicitado/gerado para a Unidade ou Unidade + Cliente, não será exibido o link para Gerar Excel e Gerar PDF.&#x20;

Será apresentado o botão "Fazer Consolidação" para que o usuário possa solicitar a consolidação do faturamento do período desejado.

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="danger" %}
<mark style="color:red;">É importante ressaltar que o "Faturamento Em Aberto" é uma pré-consolidação da quantidade a faturar para os serviços do contrato a partir da última fatura até o dia solicitado.</mark>
{% endhint %}

Ao clicar em "Fazer Consolidação", o relatório não ficará disponível imediatamente, duranto o processo de geração do relatório, o sistema apresenta uma mensagem informando que o processo ainda não foi concluído e o botão "Fazer consolidação" é substituído pelo botão "Refazer a Consolidação", que ficará inativo enquanto o relatório é gerado.

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Concluído o relatório, o usuário terá duas opções para visualização:

**Gerar Excel:** Os dados são exportados para a máquina do usuário em um arquivo em Excel.

**Gerar PDF:** Os dados são apresentados em uma nova aba do navegador em um arquivo em PDF.

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Quando o usuário aciona o botão "Refazer a Consolidação", a aplicação retoma a geração de um novo relatório de faturamento e durante esse processo não exibe os links para **Gerar Excel** e **Gerar PDF** na tela. No lugar é apresentada uma mensagem informativa do processo e ao concluir os links voltama ser exibidos ao usuário com o relatório gerado.

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>



{% hint style="danger" %}
<mark style="color:red;">Quando acionada a opção de "Fazer a Consolidação/Refazer a Consolidação" para a Unidade sem informar o cliente, será gerado um relatório consolidado com todo faturamento "Em Aberto" de todos os clientes da unidade.</mark>&#x20;

<mark style="color:red;">A consolidação destes dados exige um processamento maior para realização de cálculos da quantidade a faturar dos serviços dos contratos, portanto o tempo de disponibilização pode ser entre 10 e 20 minutos a depender da quantidade de clientes e serviços a faturar.</mark>
{% endhint %}
