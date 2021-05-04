## Programa Full Cycle de Aceleração - Edição Docker

#### Desafio 1

##### Instruções:

Para executar o desafio, siga os seguintes passos:

1. Crie uma rede para o desafio 1

```sh
docker network create desafio1
```

2. Rode o mysql

```sh
docker run --rm -d --network desafio1 --name mysql ajvideira/pfa-docker-desafio1-mysql
```

3. Rode o node

```sh
docker run --rm -d --network desafio1 --name node ajvideira/pfa-docker-desafio1-node
```

4. Rode o nginx na porta 8080

```sh
docker run --rm -d --network desafio1 -p 8080:80 --name nginx ajvideira/pfa-docker-desafio1-nginx
```

5. Acessar pelo navegador o endereço http://localhost:8080

#### Desafio 2

##### Instruções:

Para executar o desafio 2, siga os seguintes passos:

1. Clone o projeto

```sh
git clone https://github.com/ajvideira/pfa-docker.git
```

2. Entre na pasta desafio2

```sh
cd desafio2
```

3. Rode o docker-compose

```sh
docker-compose up
```

4. Acessar pelo navegador o endereço http://localhost:8000
