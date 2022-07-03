# postman-example

Exemplo de um modelo para automação de testes utilizando postman para criação de testes automatizados e o newman como executor dos testes no CI.

# Como rodar

## Instale as dependências
```
npm install -g newman
npm install -g newman-reporter-htmlextra
```

## Rodando os testes

Rodando os testes com Resultado em html e interface mais agradável, depois de rodar sera criado uma pasta testResults e dentro dela terá o report basta clicar nele.
```
  newman run ServerRest.postman_collection.json -e automation.postman_environment.json -r htmlextra --reporter-htmlextra-export testResults/htmlreport.html  
```
Rodando os testes com resultado no próprio terminal
```
  newman run ServerRest.postman_collection.json -e automation.postman_environment.json -r cli  
```


# Como importar os testes
