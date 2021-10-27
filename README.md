<p align="center">
  <a href="https://www.docker.com/" target="blank"><img src="https://seekvectorlogo.com/docker-vector-logo-svg/" width="320" alt="Docker Logo" /></a>
</p>
<br>
<br>
<p align="center">
  <a href="https://konghq.com/kong" target="blank"><img src="https://2tjosk2rxzc21medji3nfn1g-wpengine.netdna-ssl.com/wp-content/uploads/2018/08/kong-combination-mark-colors.svg" width="320" alt="Nest Logo" /></a>
</p>

## Descrição

Criação de um ambiente local para implementação e testes da API Gateway Kong.

O arquivo docker-compose é baseado no repositório https://github.com/codeedu/apigateway-kong do Wesley Williams.

Ao amadurecer dos estudos, gostaria de adicionar serviços de exemplos com NestJS (framework que utilizo) e também o Keycloak com um passo a passo de integração entre Kong e Keycloak.


## Iniciando com o Kong

Os requisitos iniciais para dar inicio aos testes, é ter o Docker e o docker-compose instalado no PC.
Durante todos os testes e futuras implementação estarei usando o Ubuntu como sistema operacional.
Link para download: https://ubuntu.com/download/desktop

Atenção!

Antes de rodar o docker-compose é necessário criar uma network no docker para abrigar o Kong, o Konga (GUI da API Gateway) e o Postgres como banco de dados para o Konga.

## Criando network do Kong

```bash
# network kong-net no Ubuntu
$ sudo docker network create kong-net
```

## Rodando docker-compose

```bash
# network kong-net no Ubuntu
$ sudo docker-compose up -d
ou
$ sudo docker-compose up
```

Lembrando que o termo -d ao final do "up" é somente para ele criar o serviço do Docker e rodar em segundo plano sem a necessidade de deixar um terminal aberto