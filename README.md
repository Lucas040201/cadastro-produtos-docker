<h3 align="center">Ac 03</h3>

> Lucas Mendes e Lucas Avelino

## 📝 Sumário

- [Como Rodar](#como)
- [Banco de dados](#banco)

## 🧐 Como Rodar <a name = "como"></a>

<p> Para rodar este projeto apenas digite no terminal docker-compose up.</p>

## 🔧 Banco de dados <a name = "banco"></a>

<p>O docker ira subir o banco de dados, portanto, é necessário apenas criar o banco de dados com os seguintes comandos:</p>

<p>Para acessar o container de mysql:</p>

    docker exec -it cadastro-produtos-docker_db_1  /bin/bash

<p>Após isso, logue no mysql e digite a senha assim que solicitar.</p>

    mysql -uroot -p


<p>Para criar o banco de dados utilize os seguintes comandos. Apenas copie e cole.</p>

    CREATE DATABASE atividade;

    USE atividade;

    CREATE TABLE usuario(
        id_produto INT  NOT NULL AUTO_INCREMENT,
        nome VARCHAR(100),
        categoria VARCHAR(100),
        preco DECIMAL,

        PRIMARY KEY (id_produto)
    );

