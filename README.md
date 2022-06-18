
# API REST Forum

Projeto simulando uma API REST de um forum de cursos

## Funcionalidades

- Autenticação e roles de usuário e administrador
- Paginação e Sort na busca de resultados
- CRUD de tópicos



## Requisitos

Para buildar e rodar a aplicação, você irá precisar de:

- [Docker](https://www.docker.com/get-started/)

## Stack utilizada

**Tech:** Java, JUnit 5, Spring Boot, Spring Security, Swagger, Maven, Docker


## Acesso

*Para acessar o projeto, faça requests para:*
https://rafael-forum.herokuapp.com/topicos

*Para obter a documentação completa da API, acesse:*
 https://rafael-forum.herokuapp.com/swagger-ui/index.html
    
## Deploy

Para fazer o deploy desse projeto, execute o seguinte comando

```bash
  docker run  -e SPRING_PROFILES_ACTIVE='prod' -p 8080:8080 -e FORUM_DATABASE_URL='jdbc:h2:mem:alura-forum' -e FORUM_DATABASE_USERNAME='sa' -e FORUM_DATABASE_PASSWORD='' -e FORUM_JWT_SECRET='123456' rafael/forum
```

