# 🏭 Produção

O menu Produção refere-se ao módulo ArqIndex do ArqGED. Este menu refere-se à configuração do processo de indexação dos documentos, como controle de filas de trabalho, configuração das etapas de indexação e possíveis correções de documentos digitalizados.&#x20;

Quando os documentos de um cliente são digitalizados por este menu, é possível acompanhar todo o processo de digitalização, desde a criação dos documentos, indexação dos metadados e sua exportação para a aplicação ArqGED.&#x20;

A indexação é o processo de cadastrar os metadados de identificação de um documento a partir de sua imagem escaneada. Essa indexação é realizada pelos operadores do setor de produção por meio de uma tela deste menu, possibilitando controle das filas de indexação dos documentos por árvore documental, cliente, código de caixa ou algum outro controle específico do gestor por meio de filtros de campos existentes na tela.&#x20;

{% hint style="info" %}
<mark style="color:blue;">**1º -**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Para cada documento digitalizado é gerada uma imagem em um arquivo XML conforme a configuração do scanner. O arquivo XML pode conter um ou mais documentos digitalizados. Esses arquivos gerados são armazenados em uma pasta configurada na aplicação ArqIndex como "Local dos Arquivos de Entrada".</mark>   &#x20;

<mark style="color:blue;">**2º -**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">A aplicação ArqIndex por meio do processo de Leitura do XML encontra o arquivo XML, realiza a validação e o processamento dos documentos e os envia para a fila de indexação conforme a configuração do fluxo.</mark>&#x20;

<mark style="color:blue;">**3º -**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Por meio do menu Produção um colaborador da Unidade terá acesso aos documentos criados e suas respectivas imagens para indexação.</mark>&#x20;

<mark style="color:blue;">**4º -**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">No processo de indexação é feito o cadastro dos dados de cada um dos documentos a partir das informações da imagem, ou seja, o operador abre um documento, visualiza sua imagem e preenche os metadados conforme os campos configurados para a árvore documental, como por exemplo nome, matrícula, CPF ou CNPJ, entre outros.</mark> &#x20;
{% endhint %}

***

## Pré-requisitos para a utilização do ArqIndex&#x20;

1. [Serviço ArqIndex](../cliente/contratos/aba-servico/regras-de-faturamento-por-tipo-de-servico.md#arqindex) no contrato da unidade/cliente, devidamente cadastrado no menu [Cliente > Contratos](../cliente/contratos/) (esse serviço é responsável pelo acesso às configurações da aplicação ArqIndex). &#x20;
2. [Serviço ArqStorage Total](../cliente/contratos/aba-servico/regras-de-faturamento-por-tipo-de-servico.md#arqstorage-total) ou [ArqStorage Ativo](../cliente/contratos/aba-servico/regras-de-faturamento-por-tipo-de-servico.md#arqstorage-ativo) no contrato da unidade/cliente, devidamente cadastrado no menu [Cliente > Contratos](../cliente/contratos/) (esse serviço é responsável pelo processo de exportação dos documentos indexados para o ArqGED).&#x20;
3. [Parâmetros Gerais ](configuracoes/parametros-gerais.md)configurados para a unidade ou cliente. Os parâmetros gerais são a identificação da configuração de funcionamento dos processos da aplicação ArqIndex. Somente após criada esta configuração será possível seu relacionamento com a aplicação ArqIndex para que então sejam realizadas as configurações de pastas para o "Local dos Arquivos de Entrada", "Local dos Arquivos em Processo" e "Local dos Arquivos em Exportação". Essa configuração é realizada no menu [Produção > Configurações > Parâmetros Gerais](configuracoes/#parametros-gerais).&#x20;
4. Fluxo de trabalho criado para a unidade ou cliente no menu [Produção > Configurações > Fluxo de Trabalho](configuracoes/#fluxo-de-trabalho). A aplicação ArqIndex utiliza o fluxo de trabalho para identificar as etapas que serão utilizadas para processamento dos documentos.&#x20;
5. Usuário do cliente ou unidade com a permissão ArqIndex devidamente parametrizada na tela [Administração > Usuários > Aba Permissões I ](../administracao/usuarios.md)> Perfil de acesso: Gestão ArqINDEX.&#x20;
6. Definição das [árvores organizacionais](../arvore-documental/arvore-organizacional.md) com os respectivos campos customizados ou de lista que serão utilizados para digitalização ou indexação dos documentos..&#x20;
7. Definição dos Id's da Unidade, do Cliente, dos campos customizados ou campos de lista e dos Id's das árvores organizacionais que serão utilizados para digitalização e indexação.&#x20;
8. Códigos de caixa para as indexações do tipo guarda terceirizada ou guarda interna. &#x20;

{% hint style="warning" %}
<mark style="color:orange;">**Os requisitos para utilização do ArqIndex dependem também do scanner que será utilizado pela unidade ou pelo cliente. É importante lembrar também que o ArqIndex é recomendado para a digitalização de documentos em grande escala. Para digitalizar uma quantidade menor de documentos, o ideal é utilizar o**</mark> [<mark style="color:blue;">**módulo ArqScan**</mark>](../documento/explorar/modulo-arqscan.md)<mark style="color:orange;">**.**</mark>
{% endhint %}

O menu Produção é composto pelos seguintes submenus:&#x20;

<table data-view="cards"><thead><tr><th align="center"></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td align="center"><mark style="color:green;"><strong>Cadastrar</strong></mark></td><td><a href="cadastrar.md">cadastrar.md</a></td></tr><tr><td align="center"><mark style="color:green;"><strong>Configurações</strong></mark></td><td><a href="configuracoes/">configuracoes</a></td></tr><tr><td align="center"><mark style="color:green;"><strong>Correção do XML</strong></mark></td><td><a href="correcao-do-xml.md">correcao-do-xml.md</a></td></tr></tbody></table>
