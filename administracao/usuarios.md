# 🟩 Usuários

No menu Usuários são criados todos os usuários que utilizam o sistema ArqGED e atribuídas as permissões de acesso às funcionalidades do sistema. &#x20;

<figure><img src="../.gitbook/assets/admin4.png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

## Criar novo usuário

<figure><img src="../.gitbook/assets/image (51).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Empresa:** Selecione o nome do cliente que deseja.

**Adicionar:** Clique para criar um novo usuário.

### Aba Usuário

<figure><img src="../.gitbook/assets/image (52).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Nome:** Informe o nome completo do usuário.

**Usuário:** Informe qual será o usuário que deverá ser utilizado na tela de acesso ao sistema.

{% hint style="info" %}
<mark style="color:blue;">Crie um padrão de usuário para seu cliente, como por exemplo: "nome" + "." + "sobrenome" (maria.santos), ou utilize o e-mail corporativo, assim será muito difícil criar um usuário já existente. Quando isso acontece, é apresentada a seguinte mensagem:</mark>

![](<../.gitbook/assets/image (53).png>)

<mark style="color:blue;">Outro ponto importante é que a validação de duplicidade de usuário ocorre em todo o banco de dados do ArqGED e não somente na base de determinado cliente.</mark>
{% endhint %}

**Tipo de Acesso:** No caso de usuário de cliente, a única opção disponível é "Cliente", quando o processo é realizado pela Unidade, também é apresentada a opção de acesso "Unidade".

**Status:** Indica a situação do usuário no sistema. Ao adicionar um novo usuário, será mantido como "**Inativo" até que sejam aplicadas todas as permissões/configurações do usuário.** Ao finalizar todas as configurações, retorne na aba de usuário e altere o status para "ativo", caso contrário, o usuário não conseguirá logar no sistema.

**Telefone Fixo e Telefone Celular:** Não são campos de preenchimento obrigatório, porém, estão disponíveis para uso.

**E-mail:** Informe o e-mail mais acessado pelo usuário, este endereço será utilizado para todo o processo de comunicação com o usuário dentro do ArqGED.

**Senha e Confirmar Senha:** Crie uma senha temporária para o usuário considerando os critérios apresentados pelo sistema: _"A senha deve conter no mínimo 8 caracteres, contendo letra maiúscula, minúscula, número e caractere especial."_

**Inativar o usuário depois do dia:** Deve ser utilizado quando o usuário precisar de acesso ao sistema por um determinado período. Ao informar uma data de inativação, automaticamente o usuário será inativado na data previamente cadastrada.&#x20;

**Alterar senha no próximo login:** Marcando o _checkbox_**,** assim que o usuário acessar o sistema pela primeira vez com a senha temporária criada para primeiro acesso, ele deverá criar uma senha pessoal considerando os critérios exigidos pelo sistema.

**Trocar senha a cada \_\_\_ mês:** Marcando o _checkbox_, o sistema deverá de forma automática solicitar o cadastro de uma nova senha, sempre que atingido o prazo estipulado.

**Notificação TTD:** Marcando o _checkbox_, o usuário será notificado quanto ao vencimento dos documentos da sua empresa, caso contratado o serviço.

{% hint style="info" %}
<mark style="color:blue;">É indicada a utilização do</mark> <mark style="color:blue;"></mark>_<mark style="color:blue;">checkbox</mark>_ <mark style="color:blue;"></mark><mark style="color:blue;">"Notificação TTD" apenas para os usuários com permissão de acesso completo a Árvore Documental do cliente, visto que para esta notificação, o sistema não valida o acesso do nível da Árvore Documental sendo o relatório de documentos vencidos enviado na íntegra ao usuário.</mark>
{% endhint %}

### Aba Permissões I

<figure><img src="../.gitbook/assets/image (54).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Master:** Informe se o usuário é do tipo Master, ou seja, se ele deve acessar a Árvore Documental completa, sendo necessário neste caso definir somente o perfil de acesso.

Quando é necessária a restrição do usuário por departamento ou tipo documental, ele não poderá ser considerado um usuário Master.

<figure><img src="../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>
