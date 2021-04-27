# pfa-docker

Programa Full Cycle de Aceleração - Edição Docker

Desafio 1

Instruções:

Para executar o desafio, siga os seguintes passos:

1. Clone o projeto

```sh
git clone https://github.com/ajvideira/pfa-docker.git
```

2. Crie uma rede para o desafio 1

```sh
docker network create desafio1
```

3. Rode o mysql

```sh
docker run --rm -d --network desafio1 --name mysql ajvideira/pfa-docker-desafio1-mysql
```

4. Rode o node

```sh
docker run --rm -d --network desafio1 --name node ajvideira/pfa-docker-desafio1-node
```

5. Rode o nginx na porta 8080

```sh
docker run --rm -d --network desafio1 -p 8080:80 --name nginx ajvideira/pfa-docker-desafio1-nginx
```

6. Acessar pelo navegador o endereço http://localhost:8080
