# Webhook

{% hint style="success" %}
É uma tecnologia que permite a comunicação entre aplicações, enviando dados automaticamente entre elas via HTTP. Os webhooks são ativados por eventos específicos (gatilhos).

Os webhooks são úteis para: Automatizar processos, Melhorar o fluxo de trabalho, Economizar recursos e custos do servidor, Integrar com serviços de terceiros e outras APIs externas.

Os webhooks são semelhantes as APIs, que permitem a comunicação entre aplicativos, mas funcionam de forma diferente. Uma API é um conjunto de protocolos e rotinas para construir e interagir com aplicativos de software, enquanto um webhook é uma forma de um aplicativo notificar outro quando ocorre um evento específico.
{% endhint %}

Este menu permite ao cliente configurar Webhooks para acompanhar o andamento dos seus processos de assinaturas de documentos.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FnFDvc7N8KjNAnPi3OCgN%252Fimage.png%3Falt%3Dmedia%26token%3Dacf3fbc9-8595-40d8-b991-b96c3e3aa66e&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=711ae1a3&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Conforme a configuração de Webhook realizada, o cliente recebe os dados de execução dos processos de assinatura por meio dos eventos/gatilhos.

Este menu é exibido aos usuários com perfil de **Administrador Global** com devida **permissão definida** na plataforma e com **plano de assinatura vigente** ou seja com **conta de status Ativo**.

Clicando em Webhook, é apresentado o GRID com as configurações de Webhook da conta do usuário logado, ordenados alfabeticamente pela coluna "Nome".

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FB3GXVCLXRPMnQjPj2Ujz%252Fimage.png%3Falt%3Dmedia%26token%3Dd3352498-4df3-4b2f-bc89-823a81483e4e&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=41252b40&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**Documentação Webhook:** Clique para acessar o detalhamento das configurações e uso do Webhook.

**Adicionar:** Utilize para incluir uma nova configuração. Ao clicar no ícone "Adicionar", a aplicação verifica o status da conta e a quantidade de configurações que a conta possui.

Somente **conta com status Ativo** pode adicionar configuração de Webhook, **limitados a 25 configurações**.

Se Conta Ativa e **possui 25 configurações de webhook**, a aplicação exibe a mensagem: **"A conta atingiu o limite máximo de X configurações de webhook."**

Se **Conta bloqueada,** a aplicação exibe a mensagem: **"A conta está bloqueada. Somente conta com status Ativo pode adicionar configuração de webhook."** .

**Excluir:** Utilize para excluir uma configuração. O ícone de exclui é habilitado somente após selecionar uma ou mais configurações de webhook com **status inativo** e que **não esteja em edição por outro usuário**.

Não é permitido excluir configuração, inativo, de webhook que estejam em edição por outro usuário.

**Filtrar:** Utilize para filtrar configurações específicas. O sistema permite ao usuário filtrar por dados contidos no resultado da consulta do GRID e não somente na página, em questão.

* Nome: permite filtrar pelo nome do webhook.
* Status: permite filtrar pelo status do webhook. O sistema lista as opções "**Ativo**", "**Inativo**" e "**Inativo por falhas**".

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252F2uZLKGVndq44TuJQcrIc%252Fimage.png%3Falt%3Dmedia%26token%3D4b3dbf06-1ba4-4114-9461-5b11591e0797&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=9551189b&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**Coluna Id:** Exibe o Id do Webhook no sistema.

**Coluna Nome:** Exibe o nome do Webhook no sistema. Quando o webhook estiver em edição, o sistema sinaliza com a informação **"Em edição com: \[Nome do usuário que está editando o webhook]".**

**Coluna Status:** Exibe o status do webhook: **Ativo**, **Inativo** ou **Inativo por falhas.**

Quando o status for "**Ativo**", ele pode ter as seguintes flags:

* **Gatilho Inativo:** Quando pelo menos um gatilho da configuração está inativo por falhas recorrentes.
* **Falha em Gatilho:** Quando não existem gatilhos inativos na configuração, mas pelo menos um gatilho tem a quantidade de falhas maior do que zero.

**Coluna Ações:** Este botão é exibido:

* Desabilitado para configurações de webhook com flag "Em edição" com outro usuário.
* Habilitado para\* configurações de webhook sem flag "Em edição" com o usuário logado.

Quando habilitado, o sistema lista as ações, conforme status do webhook: Ativar, Editar, Excluir , Inativar.

* **Ativar:** somente para configuração de webhook com status Inativo.
* **Editar:** listada para todos os webhooks.
* **Excluir:** somente para configuração de webhook com status Inativo.
* **Inativar:** somente para configuração de webhook com status Ativo.

***

## Configurações de Webhook <a href="#configuracoes-de-webhook" id="configuracoes-de-webhook"></a>

Ao clicar em Adicionar "+", é apresentada a tela para configuração de webhook.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FGbAuV6TMxC0f757FevTC%252Fimage.png%3Falt%3Dmedia%26token%3Dc679db37-1e5b-4bd5-b7a0-01fa77ee8af4&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=3cd831e5&#x26;sv=2" alt=""><figcaption></figcaption></figure>

### Dados Gerais <a href="#dados-gerais" id="dados-gerais"></a>

Os dados gerais do webhook devem ser informados nesta área:

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FxiV21TWe6L2bf3iCqUSG%252Fimage.png%3Falt%3Dmedia%26token%3D4a71ff16-da91-452f-89dd-cc25192c602a&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=8f3e4548&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**Status:** São exibidas na lista as opções "Ativo" e "Inativo", sendo exibida por padrão o preenchimento da opção "Ativo".

Na visualização/edição de um webhook já criado, caso seu status seja "Inativo por falhas", ele irá abrir na tela de configurações com o status "Inativo".

**Nome:** Informe o nome do webhook. Trata-se de um campo de preenchimento obrigatório. O sistema não permite webhooks com mesmo nome na mesma conta.

**URL para publicar:** Informe a URL que será chamada para receber os dados do processo de assinatura dos documentos. Trata-se de um campo de preenchimento obrigatório.

**Aguardar retorno:** Defina se o webhook deve aguardar um retorno. Trata-se de um campo de preenchimento opcional.

A marcação desse campo fará com que o webhook aguarde uma confirmação do seu listener (URL para publicar) após enviar uma mensagem. O webhook registra uma transferência de mensagens bem-sucedida quando o listener retorna um código de status HTTP 200. Se esta opção não é marcada e o webhook não receber um código de status HTTP 200, a aplicação não considerará isso como falha.

### Executar o webhook quando <a href="#executar-o-webhook-quando" id="executar-o-webhook-quando"></a>

Nesta área devem ser definidos os pré-requisitos para a execução do webhook.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FUvK98jk0LnmAUVOXqt3Q%252Fimage.png%3Falt%3Dmedia%26token%3Dce25cdb0-411d-42f7-8405-a3d9268cb7fe&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=e224723e&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**Adicionar Grupos e Usuários**

Esta opção é utilizada para configurar um ou mais grupos e/ou usuários como parâmetro de execução do webhook. Ou seja, o webhook somente será executado se o remetente do processo for um usuário selecionado ou se fizer parte de um grupo configurado neste campo. Trata-se de um campo de preenchimento opcional.

Caso um dos grupos listados tiver sido excluído posteriormente, ele será apresentado em vermelho.

Caso um dos usuários listados tiver sido inativado, bloqueado ou deixado de ser administrador global posteriormente, ele será apresentado em vermelho.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252F9at5gnvVv3Tdu0VHfsWG%252Fimage.png%3Falt%3Dmedia%26token%3D8dd0e2e4-b63e-4e26-9de6-87b0e96c6a21&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=11de7299&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Do lado direito da tela são apresentados os "Grupos" e os "Usuários" disponíveis para seleção. Do lado esquerdo da tela são apresentados os "Grupos" e os "Usuários" já selecionados.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252F5fAinFg4evP72PSqUOqo%252Fimage.png%3Falt%3Dmedia%26token%3Df0e0a291-c25a-42bf-8147-a3ce85e00fab&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=1c6ccaf9&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Utilize os botões disponíveis, clique sobre o nome do grupo ou nome do usuário que deseja mover e depois clique nos botões para "Adicionar", para envio de um por vez ou "Adicionar todos" para envio da lista completa. O mesmo deve ser feito para "Remover" itens da lista.

Concluída a seleção dos usuários e grupos, clique "Selecionar" para retornar a tela anterior.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FcBO16CymwSoRVnewdMIq%252Fimage.png%3Falt%3Dmedia%26token%3Dddd9311f-d795-45ec-bcc9-ae1f46cf8d36&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=4e620739&#x26;sv=2" alt=""><figcaption></figcaption></figure>

As definições realizadas serão apresentadas no campo "**O processo tenha sido enviado por algum usuário do grupo ou usuário selecionado neste campo**", que é verificado para "**Execução do webhook**".

**Adicionar pastas**

Esta opção é utilizada para configurar uma ou mais pastas como parâmetro de execução do webhook. Ou seja, o webhook somente será executado caso o processo tenha sido criado em alguma pasta contida neste campo. Neste campo serão exibidas as pastas selecionadas na modal "Pastas". Trata-se de um campo de preenchimento opcional.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FzIJ6UjzlMqlHuClDA4Gb%252Fimage.png%3Falt%3Dmedia%26token%3D16babba3-8603-4f98-899a-6fc28db1a77a&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=d6ec0c64&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Selecione na árvore apresentada a pasta que deseja limitar a execução do webhook. No campo "Pastas selecionadas" serão listadas todas as pastas marcadas. Clique "Selecionar" para concluir a configuração.

Caso uma das pastas listadas tenha sido excluída posteriormente, ela será apresentada em vermelho.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FoJ1RfyYLGEhsaPfHo9aO%252Fimage.png%3Falt%3Dmedia%26token%3Dfad09d74-581f-4bc9-a87b-8cacd453d3d4&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=9dc76086&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Leia com atenção a mensagem de validação do processo e clique para prosseguir.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252F81FqRR3ROJ6SkRIJD4Ab%252Fimage.png%3Falt%3Dmedia%26token%3D81eb68e3-c397-47b5-aeb7-7cbc8c572d1d&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=27ced95b&#x26;sv=2" alt=""><figcaption></figcaption></figure>

As definições realizadas serão apresentadas no campo "**O processo tenha sido criado em uma das pastas selecionadas neste campo**", que é verificado para "**Execução do webhook**".

### Gatilhos <a href="#gatilhos" id="gatilhos"></a>

Nesta área, é necessário definir um ou mais gatilhos de execução do webhook. Ou seja, aqui são definidos os momentos em que o webhook será executado, chamando a URL com os dados no JSON, conforme configuração de retorno.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FrLzmZPtcJWAy6FY6JEXg%252Fimage.png%3Falt%3Dmedia%26token%3D76a5a988-4103-488f-bc55-a3fe74bcc3c1&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=32ab6d4e&#x26;sv=2" alt=""><figcaption></figcaption></figure>

É obrigatória a seleção de ao menos um gatilho para execução do webhook, são apresentadas as seguintes opções:

1. Processo enviado
2. Processo com falha de envio
3. Processo assinado por algum signatário
4. Processo recusado por algum signatário
5. Processo cancelado pelo remetente
6. Processo expirado
7. Processo reenviado
8. Processo assinado/concluído por todos os signatários

### Retorno <a href="#retorno" id="retorno"></a>

Nesta área, são definidos os dados que serão retornados no JSON, além dos dados gerais.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FTNf5Aq2eHmTpqvbIm66q%252Fimage.png%3Falt%3Dmedia%26token%3D62d609bd-2b21-46f8-b83d-246a85ef9af2&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=3cf4ed06&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Os possíveis dados são:

* **Processo:** Parte do JSON com os dados do processo;
* **Signatários:** Parte do JSON com os dados dos signatários;
* **Documentos:** Parte do JSON com os dados dos documentos do processo.

Os dados gerais fazem parte do início do JSON e esta parte será enviada sempre, mesmo se não houver nenhum dado marcado de retorno para o JSON.

### Json <a href="#json" id="json"></a>

Nesta área, o sistema exibe o exemplo de retorno do JSON.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FqMpuixxyCI4WaMHd1M4o%252Fimage.png%3Falt%3Dmedia%26token%3Dcd252e9d-8caa-4807-8d83-50317a646a87&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=e270cb32&#x26;sv=2" alt=""><figcaption></figcaption></figure>

O dados de retornos configurados, são representados no campo JSON a medida que os campos são marcados.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FH8w9bU8L4yvALmvNsyWL%252Fimage.png%3Falt%3Dmedia%26token%3D3eb43eca-f899-4aa1-8899-c873cfb92576&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=32eba280&#x26;sv=2" alt=""><figcaption></figcaption></figure>

* Ao marcar o campo "**Dados do processo**”, o sistema exibe o exemplo dos dados do processo no campo "JSON".
* Ao marcar o campo "**Signatários**", o sistema exibe o exemplo dos dados dos signatários no campo "JSON".
* Ao marcar o campo "**Documentos**", o sistema marca checkbox "Arquivos do processo", "Link dos documentos compartilhados" e "Registro de assinatura".

"**Arquivos do processo**" e “**Registros de assinatura**" podem ser retornados no formato Link para Download ou Base64. É necessário marcar uma opção de formado para os arquivos do processo e/ou registros de assinaturas

O "**Link dos documentos compartilhados**" é o link de compartilhamento dos documentos do processo. Estes links são disponibilizados somente na conclusão de processos que possui a configuração "**GerarQRCode**". Concluídas as configurações, clique "Salvar". Serão habilitadas novas abas para andamento das configurações.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252F3v3WE9zf2LSL7vneV9QW%252Fimage.png%3Falt%3Dmedia%26token%3D0f594a3b-9feb-431c-a8f0-9748e85283c7&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=fbc85ce7&#x26;sv=2" alt=""><figcaption></figcaption></figure>

***

## HMAC <a href="#hmac" id="hmac"></a>

Toda configuração realizada na plataforma terá uma chave HMAC gerada. Para visualizar, clique na aba HMAC.

**HMAC** é uma forma de verificar a autenticidade e integridade das informações que estão sendo transmitidas por meio de uma chave secreta compartilhada entre as partes.

A cada webhook gerado na ArqSIGN, a aplicação irá gerar o “**Chave secreta HMAC**”. Esta chave será de conhecimento somente da ArqSIGN e da aplicação do cliente.

A “**Chave secreta HMAC**” e o body da requisição devem ser usados para o cálculo do SHA256 HMAC hash. Este hash será enviado no cabeçalho da requisição como “**HMAC**”.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FgeiqvYH5dLomPOeKYAJt%252Fimage.png%3Falt%3Dmedia%26token%3D26bd579c-bc3f-431b-9732-7077930115dc&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=b6331612&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Utilizando os ícones disponíveis na tela, o usuário poderá:

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252Fu9GfjylXJJ8FSMJLjRYZ%252Fimage.png%3Falt%3Dmedia%26token%3D3ecdefa2-7cf8-46e0-b939-7f8d98c8a4b8&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=5a339d47&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**Visualizar:** Ao clicar no ícone, a chave HMAC é apresentada na tela.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FENsfinr4SrnsipbwVdMn%252Fimage.png%3Falt%3Dmedia%26token%3D7f49a72d-2f5f-4d58-baee-ddd4c313480c&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=a994c2ff&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**Copiar:** Após clicar no ícone de visualização, é habilitada a opção de "Copiar" a chave HMAC.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FoqR5hqprsy59LG4XxDgI%252Fimage.png%3Falt%3Dmedia%26token%3D905c1c7b-3192-42ba-9dee-c6f3e582ff22&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=b7959acb&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**Regerar Chave:** Ao clicar nesta opção, uma nova chave HMAC é gerada pelo sistema.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FbKrNWc4PZGAs6ti5fDDI%252Fimage.png%3Falt%3Dmedia%26token%3D635b2ecf-2b11-437d-a125-f0044fb71fc0&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=8eb4a606&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Valide a ação na tela para prosseguir.

***

## Gatilho <a href="#gatilho" id="gatilho"></a>

Nesta são listados os gatilhos configurados para o webhook, em questão, ordenados conforme evento de execução.

Uma configuração de webhook pode ater até 8 gatilhos:

1. Processo enviado
2. Processo com falha de envio
3. Processo assinado por algum signatário
4. Processo recusado por algum signatário
5. Processo cancelado pelo remetente
6. Processo expirado
7. Processo reenviado
8. Processo assinado/concluído por todos os signatários

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252F8uPFmm12RFrldCCagD8G%252Fimage.png%3Falt%3Dmedia%26token%3Dc4e9d7e1-e4ee-415b-9264-6acf74a03a08&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=936787dc&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**Gatilhos do Webhook:** Traz o nome informado na tela de configuração para o processo.

**Coluna Gatilho:** Lista os gatilhos selecionados na tela de configuração.

**Coluna Quantidade de Falhas:** O sistema exibe a quantidade de falhas registradas para cada gatilho, quando houver.

**Coluna Status:** Mostra o status de cada gatilho.

Para gatilhos com status "**inativo por falhas recorrentes"** e que não esteja em edição por outro usuário, o sistema exibe o botão "**Ativar**" habilitado, possibilitando ao usuário ativar o gatilho novamente.

Ao reativar o gatilho que está inativo por falhar recorrentes, o sistema zera a contagem de falhas.

**Coluna Ações:** Permite nova ativação de um gatilho inativado por falhas recorrentes, desde que não haja nenhum outro usuário realizando a edição do gatilho em questão.

### Execução <a href="#execucao" id="execucao"></a>

A cada evento na aplicação, conforme os gatilhos listados abaixo, o sistema executa o webhook, enviando atualizações (mensagens de evento) para a URL configurada em tempo real, ou seja, no ato da ocorrência do evento configurado.

1. **Processo enviado:** Ao enviar um processo pela aplicação ArqSign ou API, o sistema executa o webhook com este gatilho, enviando os dados, conforme a configuração de retorno, para a URL configurada.
2. **Processo com falha de envio:** Quando houver falha de envio do processo para algum destinatário e/ou falha de envio do código de segurança para algum destinatário.

O Retorno do JSON quando marcado para retornar os dados “Signatários” para este gatilho em específico, retornará somente os dados do signatário que teve a falha de envio do processo e/ou código de segurança.

1. **Processo assinado por algum signatário:** Assim que o processo é assinado por cada signatário. Desta forma, se o processo possuir 3 signatários, a cada assinatura concluída o webhook com esta configuração irá chamar a URL definida e ao final do processo de assinatura a URL terá sido chamada 3x.

O Retorno do JSON quando marcado para retornar os dados “Signatários” para este gatilho em específico, retornará somente os dados do signatário que assinou os documentos.

1. **Processo recusado por algum signatário:** Assim que algum signatário se recusar a assinar algum documento.
2. **Processo cancelado pelo remetente:** Assim que o remetente do processo cancelar o seu envio.
3. **Processo expirado:** Assim que o processo expirar, ou seja, ele vencer antes da conclusão total das assinaturas.
4. **Processo reenviado:** Assim que o processo for reenviado aos signatários pendentes de assinatura. O processo pode ser reenviado quando:

* O link de assinatura expira e se deseja atualizar o link para os signatários pendentes;
* Se deseja alterar algum signatário pendente de assinatura totalmente ou apenas a forma de envio para ele;
* Se deseja reenviar o link para algum signatário mesmo que este não esteja vencido.

1. **Processo assinado/concluído por todos os signatários:** Assim que o processo é totalmente assinado por todos os signatários.

### Falhas na Execução <a href="#falhas-na-execucao" id="falhas-na-execucao"></a>

Quando o envio dos dados não é bem-sucedido, a informação de falha é registrada no sistema para uma posterior tentativa de envio de forma manual ou automatizada. A aplicação considera uma entrega bem-sucedida ou não conforme alguns parâmetros:

**A. Webhook configurado COM a opção “Aguardar Retorno”:**

Com esta configuração, o webhook aguarda, por um período de 100 segundos, uma confirmação do seu listener (URL a publicar) após o envio da mensagem.

A confirmação esperada é um código de status **HTTP 200 - OK**.

1. Se o listener não responder no **tempo esperado**, **o sistema registra como falha (tratada)**. Ou seja, a **falta de retorno é considerada uma falha que é tratada.**
2. Se o listener **retornar um código diferente de HTTP 200**, o webhook **considera que houve falha na entrega.**

As transmissões com falhas na entrega são elegíveis para novas tentativas manuais ou automatizadas, exceto as falhas com os códigos abaixo:

* 401 – Não autorizado. Existem problemas nas credenciais para acessar o HTTP.
* 403 – Sem permissão de acesso ao servidor. O servidor atendeu à solicitação, mas se recusa a fazê-la.
* 404 – URL não existe.

**B. Webhook é configurado SEM a opção “Aguardar Retorno”:**

Sem esta configuração, o webhook deve aguardar, por um **período de 100 segundos**, uma confirmação do seu listener após o envio da mensagem.

A confirmação aguardada é um código de status **HTTP 200 – OK**.

1. Se o listener não responder **no tempo esperado**, **o sistema não registra como falha. Ou seja, a falta de retorno não é considerada uma falha.**
2. Se o listener **retornar um código diferente de HTTP 200**, o webhook **considera que houve falha na entrega.**

As transmissões com falhas na entrega são elegíveis para novas tentativas manuais ou automatizadas, exceto as falhas com os códigos abaixo:

* 401 – Não autorizado. Existem problemas nas credenciais para acessar o HTTP.
* 403 – Sem permissão de acesso ao servidor. O servidor atendeu a solicitação, mas se recusa a fazê-la.
* 404 – URL não existe.

### Retransmissão em caso de falhas <a href="#retransmissao-em-caso-de-falhas" id="retransmissao-em-caso-de-falhas"></a>

As falhas de comunicação elegíveis para retransmissão poderão ocorrer de forma manual, via solicitação do usuário na aplicação ou de forma automática conforme a periodicidade abaixo:

* 1ª Tentativa: no ato do evento
* 2ª Tentativa: 05 minutos após a primeira tentativa
* 3ª Tentativa: 15 minutos após a primeira tentativa
* 4ª Tentativa: 30 minutos após a primeira tentativa
* 5ª Tentativa: 01 hora após a primeira tentativa
* 6ª Tentativa: 02 horas após a primeira tentativa
* 7ª Tentativa: 04 horas após a primeira tentativa
* 8ª Tentativa: 08 horas após a primeira tentativa
* 9ª Tentativa: 16 horas após a primeira tentativa
* 10ª Tentativa: 1º dia após a primeira tentativa
* 11ª Tentativa: 2º dia após a primeira tentativa
* 12ª Tentativa: 3º dia após a primeira tentativa
* 13ª Tentativa: 4º dia após a primeira tentativa
* 14ª Tentativa: 5º dia após a primeira tentativa, se neste dia o webhook ainda apresentar falha, então ele será inativado **(Inativo por falhas recorrentes)**.

Cada evento configurado no webhook que houver falha, terá no máximo 14 tentativas, contando com a primeira tentativa que ocorre no ato do evento.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FOw6Tf5mACZcwjo5H562j%252Fimage.png%3Falt%3Dmedia%26token%3D8208d750-166d-4586-9dcf-15af20e1d6e9&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=717e0359&#x26;sv=2" alt=""><figcaption></figcaption></figure>

### Inativação automática do webhook por falhas <a href="#inativacao-automatica-do-webhook-por-falhas" id="inativacao-automatica-do-webhook-por-falhas"></a>

Sempre que o webhook receber do listener (URL do cliente) os códigos de erros abaixo, este webhook será inativado imediatamente para evitar chamadas desnecessárias, recebendo o status “**Inativo por falhas**”.

Os códigos de erros são:

* 401 – Não autorizado. Existem problemas nas credenciais para acessar o HTTP.
* 403 – Sem permissão de acesso ao servidor. O servidor atendeu à solicitação, mas se recusa a fazê-la.
* 404 – URL não existe.

Sempre que o webhook receber outros erros diferentes dos citados acima, **após 5º dia** de erros consecutivos, o gatilho com estas falhas será inativado, recebendo o status “**Inativo por falhas recorrentes**”.

Os webhooks inativados pela aplicação por falhas, receberão os status “**Inativo por falhas**” e deixarão de enviar mensagens ao listener (URL do cliente), mas poderão ser editados e ativados novamente.

**Inativar**

Quando um gatilho for inativado por falhas recorrentes, todos os registros de falha deste gatilho que estiverem na fila de execução para serem reenviados serão removidos.

**Ativar**

Ao reativar um gatilho que foi inativado por falhas recorrentes, o sistema inclui, novamente, na fila de execução, todos os registros de falha que não atingiram as 14 tentativas de reenvio dos dados, executando o reenvio imediato dos dados da tentativa atual. As tentativas seguintes, caso existam, seguirão o tempo padrão estipulado e

Além disso, o sistema exibe a mensagem informando que registros de eventos com falha do gatilho que foi reativado, foram reenviados automaticamente.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FQ8t7jL1mHwGa7tLSqHL8%252Fimage.png%3Falt%3Dmedia%26token%3Dac18e9f0-e9b3-4c1f-9cfe-0a83e7ccced2&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=3bb551a&#x26;sv=2" alt=""><figcaption></figcaption></figure>

***

## Logs de falha <a href="#logs-de-falha" id="logs-de-falha"></a>

Nesta aba é possível acompanhar os logs de falha do webhook.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FqTqRhNO4mk8KpVznqVCb%252Fimage.png%3Falt%3Dmedia%26token%3D7a0bcd5e-d7ae-4755-aec9-05c3a1660f24&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=8dbae5c1&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Nesta tela também é possível reenviar os dados manualmente clicando no botão "Reenviar". Este botão ficará habilitado apenas se o registro não tiver atingido a 14ª tentativa.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252Fzve8wc3sXCinoLPbMYfM%252Fimage.png%3Falt%3Dmedia%26token%3De55ece0d-03e7-455e-aab4-4f1a7f5459f7&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=b0931b3b&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Se o Webhook estiver inativo ou estiver em edição por outro usuário, todos os registros do GRID terão o botão "Reenviar" desabilitado.

Ao acionar o botão \[Reenviar] o sistema executa a tentativa de envio da mensagem.

Em todos os casos, se um reenvio tiver sucesso, o registro é removido do GRID e a quantidade de tentativas do gatilho deve ser zerada.

Na coluna "Falha", é apresenta a mensagem da falha ocorrido. Ao clicar no ícone uma nova janela é aberta.

<figure><img src="https://manual.arquivar.com/manual-arqsign/~gitbook/image?url=https%3A%2F%2F2201914335-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkvKZtdmOiilgqExqFNO%252Fuploads%252FXCFbB7SIHcvPSvBqZjpi%252Fimage.png%3Falt%3Dmedia%26token%3Db000db24-5015-44aa-bd6e-a8f6d110b519&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=8e95ad55&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Na nova janela, além da mensagem de detalhamento da falha, são apresentados outros dados do processo.

**Reenviar**

É permitido o reenvio dos dados manualmente dos registros com falha somente para gatilhos com status ativo. Os registros com falha do gatilho com status inativo são listados com o botão "Reenviar" desabilitado.
