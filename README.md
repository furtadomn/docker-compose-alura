### Docker-Compose Alura

<strong>Curso Alura:</strong> [Docker: Criando containers sem dor de cabeça](https://cursos.alura.com.br/course/docker-e-docker-compose) (capítulo 6)

<strong>Instrutor:</strong> [Douglas Quintanilha](https://www.linkedin.com/in/douglas-quintanilha/)

Esta aplicação foi disponibilizada pelo curso. O capítulo 6 teve como objetivo explicar sobre a tecnologia Docker Compose, além de ilustrar a criação do arquivo docker-compose.yml e como subir os serviços.

</br>

## Como testar
Primeiramente será necessário clonar este repositório. Acesse seu terminal e execute o comando:
```
git clone git@github.com:furtadomn/imagem-docker-alura.git
```
O segundo passo é construir ("<i>buildar</i>") os serviços. Ainda no terminal, acesse o diretório do projeto clonado e execute o comando:
```
docker-compose build
```
Feito isso já é possível subir a aplicação através do comando:
```
docker-compose up
```

</br>

No navegador, acesse:
http://localhost/80

Em um primeiro momento a página estará vazia, apenas com cabeçalho e rodapé. Para exibir os livros, é preciso "alimentar" o banco de dados acessando a página http://localhost:80/seed (na qual haverá uma mensagem dizendo "Livros salvos") e retornar para http://localhost/80.

</br>

Para interromper a execusão dos containers e removê-los, execute o comando:
```
docker-compose down
```
Se o docker estiver rodando no seu terminal, dê um <strong>CTRL+C</strong> para interromper a execução (ou abra um novo terminal e digite `docker-compose stop`) e depois execute o comando acima.