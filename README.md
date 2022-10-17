# MongoDB-commerce

## Introdução

O projeto consiste em praticar e consolidar os conhecimentos aprendidos em mongoDB.

## Sumário

- [Introdução](#introdução)
- [Ferramentas utilizadas](#ferramentas-utilizada)
- [MongoDB](#mongodb)
- [Aprendizados](#aprendizados)
- [Instruções para utilizar a aplicação](#instruções-para-utilizar-a-aplicação)
- [Histórico de Commits](#histórico-de-commits)

## Ferramentas utilizada

**Back End:** Docker, MongoDB.

## MongoDB

Segundo o [Site oficial do MongoDB](https://www.mongodb.com/pt-br/what-is-mongodb), o MongoDB é um banco de dados de documentos com a escalabilidade e flexibilidade que você deseja junto com a consulta e indexação que você precisa.

## Aprendizados

Fui capaz de consolidar os conhecimentos em MongoDB, utilizando diversas queries para fazer as mais diversas consultas ao banco de dados de um restaurante. Utilizei os seguintes operadores e métodos combinados:

  * `updateOne()` e `updateMany()` para atualizar documentos.

  * Operadores `$set`, `$mul`, `$inc`, `$min`, `$max` e `$currentDate`

  * Operadores `$pop`, `$pull` e `$push`
  
  * Operador `$addToSet`

  * Operadores `$each`, `$slice` e `$sort`

  * Operador `$elemMatch` para filtrar documentos

  * Operador `$size` para filtrar documentos pelo tamanho de arrays

  * Operador `$expr` para criar expressões de agregação

## Instruções para utilizar a aplicação

Para utilizar a aplicação você precisará ter o [Docker](https://docs.docker.com/engine/install/ubuntu/) instalado e seguir os passos abaixo:

1 - Acesse o terminal na pasta raíz do projeto;

2 - Crie um container com um volume apontando para a pasta do projeto `docker run -d --name=nomeDoContainer -v "$PWD:/app" -p 27017:27017 mongo:5.0`;

3 - Com o container em execução, acesse o terminal do container `docker exec -it nomeDoContainer bash`;

4 - No terminal do container, acesse o diretório /app mapeado no volume conforme o passo 2;

5 - Por fim, execute o script de testes do projeto: `./scripts/evaluate.sh.` Se por algum motivo a execução do container for finalizada, basta iniciá-lo novamente com o comando docker start nomeDoContainer e seguir a partir do passo 3.

## Histórico de commits

Você pode verificar todo o histório de commits para saber como a aplicação foi desenvolvida passo a passo, todos eles foram feitos com base no guia de [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), mantendo uma organização e descrição objetiva do que foi feito a cada mudança!
***
  <a href="https://www.linkedin.com/in/isaacalmeidafilho/">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>

