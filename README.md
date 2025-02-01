### Esta função retorna:
As estatísticas de uso do Lambda através da função `lambda.getAccountSettings()` e retorna o objeto:
```json
{
  "TotalCodeSize": 1007,
  "FunctionCount": 1
}
```

### O Objetivo é demonstrar:
- A estrutura básica de uma função do AWS Lambda;
- Como criar permissões para o Lambda no IAM;
- Como criar uma trigger no API Gateway para chamar a função Lambda; 

### Estrutura
- `function/index.js`: Contém a função Lambda a ser executada
- `function/package.json`: Arquivo de dependências do nodejs
- `function.zip`: Versão zipada para upload

### Empacotamento da função
Esta função utiliza apenas o pacote do `aws-sdk` que não é necessário ser enviado para a AWS, mas por padrão ele é 
instalado e empacotado com a função. O conteúdo do arquivo `function/index.js` pode ser inserido diretamente no painel
do lambda sem a inclusão do diretório `node_modules`.

