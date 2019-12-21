# Docker-Compose-PostgreSQL
Dentro do *docker-compose.yml* terá a configuração e conteúdo dos serviços utilizados, no caso estaremos utilizando Docker Compose de  PostgreSQL e PgAdmin 4.

## Após configuração da imagem 
Acesse o pgadmin na porta da configurada no meu caso: [localhost:16543](http://localhost:16543/).
Digite o usuario e senha definidos no *docker-compose.yml* **PGADMIN_DEFAULT_EMAIL** **PGADMIN_DEFAULT_PASSWORD**

## Configuração para conectar pelo pgadmin
Para fazer a conexão ao banco de dados basta dentro do pgadmin.
e a senha é admin defininada no compose também.

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
