# Docker-Compose-PostgreSQL
Dentro do *docker-compose.yml* terá a configuração e conteúdo dos serviços utilizados, no caso estaremos utilizando Docker Compose de  PostgreSQL e PgAdmin 4.

## Requirimentos:
* Para utilizar em linux, você precisa do docker e do docker composer.
* Para Windows faça o download pelo [Docker Hub](https://docs.docker.com/docker-for-windows/install/).

## Para começar: (após instalação)
* Caso precise, mas não necessário, edite os acessos do docker!
* Antes de iniciar crie uma pasta junto ao *docker-compose.yml* `/database-volume`
* Abra o console no path inicie com: `docker-compose up`

## Após configuração dos serviços:
Acesse o pgadmin na porta da configurada no meu caso: [localhost:16543](http://localhost:16543/).
Digite o usuario e senha definidos no *docker-compose.yml*: `PGADMIN_DEFAULT_EMAIL` e `PGADMIN_DEFAULT_PASSWORD`

## Como conectar e configuração no pgadmin:
Para fazer a conexão ao banco de dados basta dentro do pgadmin.
* Host: `serverpostgres`
* Port: `5432`
* User: `postgres`
* Password: `admin` (definida no *docker-compose.yml*)

##### Imagem da configuração:
![Configuration](https://i.imgur.com/fEgEpIk.png)

E só aproveitar!

## Caso você esteja trabalhando com Windows 10 
Provavelmente você terá o problema “no matching manifest for windows/amd64 in the manifest list entries”
Caso ainda não tenha configurado faça os seguintes passos:

* Botão direito no docker 
* Vá em Settings
* Daemon
* Marque Advanced
* Mude o valor para "experimental": true
* Reinicie o Docker
