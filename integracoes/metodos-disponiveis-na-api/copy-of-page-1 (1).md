# ◼️ 7. Nota Fiscal

## 7.1.POST Cadastrar nota fiscal como documento: não usar este método. Usar o método POST Documento <a href="#id-7.1.post-api-notafiscal-importanotafiscal" id="id-7.1.post-api-notafiscal-importanotafiscal"></a>

### Entrada <a href="#entrada" id="entrada"></a>

• idUnidade

• idCliente

• idArvoreOrganizacional

• JSON com os dados da nota fiscal

#### **Request body**

```json
{
    "idArvore": "guid", //id da arvore organizacional
    "cnpj": "string",//cnpj da unidade prestadora de serviço do cliente
    "arquivoXML": "bytes",//byte do arquivo xml
    "arquivoPDF": "bytes",// byte do arquivo pdf
    "CamposCustomizados": {//campos customizados, conforme a configuração do idArvore informado.
        "CNPJ - Filial": "string",
        "CNPJ - Fornecedor": "string",
        "Data de Emissão Inicial": "string",
        "Data de Emissão Final": "string",
        "Data de Vencimento": "string",
        "Fornecedor": "string",
        "Natureza da Operação": "string",
        "NRO Nota": "string ",
        "Status": "string ",
        "Valor Total": "string"
    }
}
```

### Saída/Retorno <a href="#saida-retorno" id="saida-retorno"></a>

O sistema retorna o status 200 OK.

#### **Response**

```json
OK
```
