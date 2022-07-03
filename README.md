# postman-example

Exemplo de um modelo para automação de testes utilizando postman para criação de testes automatizados e o newman como executor dos testes no CI.

# Como rodar

## Instale as dependencias
```
npm install -g newman
npm install -g newman-reporter-htmlextra
```

## Rodando os testes
```
  newman run ServerRest.postman_collection.json -e automation.postman_environment.json -r cli,htmlextra --reporter-htmlextra-export testResults/htmlreport.html  
```
# Como importar os testes
