# README.md

## Teste Local no Ambiente de Desenvolvimento

1. Execute o comando `npm install` para instalar todas as dependências necessárias.
2. Inicie a aplicação localmente utilizando `node index.js` e acesse [http://localhost:8080/api-docs/](http://localhost:8080/api-docs/) para explorar a documentação da API.

## Testando a Aplicação no Ambiente Dockerizado

1. Para criar uma imagem Docker, utilize o comando `docker build -t api-conversao .`.
2. Execute a aplicação no Docker com o comando `docker run -d -p 8080:8080 api-conversao`.
3. Acesse [http://localhost:8080/api-docs/](http://localhost:8080/api-docs/) para interagir com a documentação da API.

## Criando a imagem para o Docker Hub

1. Crie a imagem usando o comando `docker build -t <seu-nome-de-usuario>/api-conversao:alpine .`.

   Exemplo: `docker build -t omaxfernandess/api-conversao:alpine .`

2. Execute a imagem com o comando `docker container run -d -p 8080:8080 <seu-nome-de-usuario>/api-conversao:alpine`.

   Exemplo: `docker container run -d -p 8080:8080 omaxfernandess/api-conversao:alpine`

3. Para enviar a imagem Docker para o Docker Hub, utilize `docker push <seu-nome-de-usuario>/api-conversao:alpine`.

   Exemplo: `docker push omaxfernandess/api-conversao:alpine`
