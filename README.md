Teste de API Rest de manual a CI/CD  

## O que é  
Este repositório foi criado como Teste de API Rest.  

## Tecnologias utilizadas 
- Postman versão web
- node version v24.12.0
- newman v6.2.1
  
## Documentações  - Doc da API: [Consulte Swagger](https://serverest.dev/#/) 

## Como instalar o ambiente 
- Primeiro: instale o node em seu computador [baixe aqui](https://nodejs.org/en/download) 
- Segundo: realize a instalação do newman de forma global. 
``` 
npm install -g newman 
```
- Terceiro: realize a instalação da dependencia dos relatórios (opcional) [newman-reporter-htmlextra 
] 
``` 
npm install -g newman-reporter-htmlextra 
``` 
## Como rodar os testes  
### Pelo Postman web ou desktop 

- Import a collection e o environment - Execute os teste de forma manual ou automatizada 

### Pelo Newman / Report  

- Abra o console de preferência - Execute a seguinte linha de comando para rodar os testes 
``` 
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli 
```
- Execute os teste com relatório 
``` 
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra 
``` 
Se você optou por rodar os teste com o report htmlextra, você gerou um arquivo html com o resultado dos testes e 
para verificar as validações, você pode abrir a pasta newman que foi criada no mesmo diretório da collection.


## Entre em contato  
email: dercioforato@gmail.com
