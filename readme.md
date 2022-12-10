<h1 align="center"> 
  Compose - Dump PostgreSQL
</h1>

Este Docker-compose, virtualiza um ambiente com o banco de dados PostgreSQL e realiza um dump data de um banco de dados externo, foi desenvolvido visando a correção rápida de um problema em uma ambiente controlado.

### :hammer_and_wrench: Tecnologias

As seguintes tecnologias e ferramentas foram utilizadas neste projeto: `Docker, Docker Compose, PostgreSQL`

### Estrutura do projeto:

```
├── db
│   └── Dockerfile
├── .dockerignore
├── .env.sample
├── .gitignore
├── docker-compose.yml
├── readme.md
```

### :gear: Como utilizar

Para consumir esta API, é preciso seguir o passo a passo abaixo.

- Tutorial para rodar o projeto

No arquivo `.env.example`, complete as variâveis com os valores do seu banco PostgreSQL e renomeie o arquivo para `.env`.

```cl
DB_HOST=
DB_PORT=
DB_USERNAME=
DB_PASSWORD=
DB_NAME=
```

Para prosseguir, é preciso que todas as ferramentas necessárias estejam devidamente instaladas (Docker, Docker Compose,...). Para conferir a instalação delas, acesse [Docker Setup](https://docs.docker.com/desktop/). Após os downloads, baixe ou clone este repositório pelo terminal seguindo passo a passo descrito abaixo:

```bash
# Baixe este repositório ou clone pelo Git usando o comando:
$ git clone https://github.com/ThHenrique/docker-dump-data.git

# Acesse a pasta do projeto
$ cd docker-dump-data

# Crie e execute a aplicação
$ docker-compose up -d
```

O Docker compose extrai uma imagem do PostgreSQL, cria uma imagem para a aplicação e inicia o serviço do PostgreSQL na porta 5432. Para consultar e gerenciar esse banco de dados criado utilize um aplicativo de sua prerência.
