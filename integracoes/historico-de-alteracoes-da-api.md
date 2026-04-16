# 🟩 Histórico de alterações da API

## 2024

<details>

<summary>28/05/2024 - Ajuste do Método GET</summary>

O método **/api/Documento/Get** da API integração, foi alterado para retornar o valor dos campos customizados dos documentos, retirando os espaços no início e no fim de campos cadastrados incorretamente, também serão removidos espaços duplos entre o conteúdo dos campos.

Foi criado o parâmetro **RemoverEspacos** que poderá ter valor **true** ou **false**, não obrigatório. &#x20;

Quando o parâmetro **RemoverEspacos** for enviado como **true**, então a API irá tratar o retorno para:&#x20;

* Retirar todos os espaços no início e no final de cada campo customizado e de lista;&#x20;
* Retirar espaços maiores que duplos entre os conteúdos dos campos customizados e de lista.&#x20;

<img src="../.gitbook/assets/image (19) (1).png" alt="" data-size="original">

Esta alteração foi criada para melhorar a integração com E-Social.

</details>
