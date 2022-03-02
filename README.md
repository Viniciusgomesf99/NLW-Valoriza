## NLW Valoriza Projeto ROCKETSEAT

## Regras

 - Cadastro de usuário

    ( ) Não é permitido cadastrar mais de um usuario com mesmo e-mail.

    ( ) Não é permitido cadastro sem email.


- Cadastro de TAG

    ( ) Não é permitido cadastrar mais de uma tag de mesmo nome.

    ( ) Não é permitido cadastrar tag sem nome.

    ( ) Não é permitido o cadastro por usuários sem permissões de administrador.

- Cadastro de elogios

    ( ) Não é permitido um usuário cadastrar um elogio para si.

    ( ) Não é permitido cadastrar elogios para usuário não existente.

    ( ) É necessário o usuário ser autenticado na aplicação.




    ## Migrations
        Migration é um arquivo com as queries SQL para atualizar o esboço do nosso BD¹ e aplicar novas mudanças a um BD existente.

        Para utilizar definimos o diretório no nosso ormconfig.json, exemplo:
        "migrations": ["src/database/migrations/*.ts"]
    ## Entities
        Entity é uma classe que tem como funcionalidade mapear as tabelas do nosso BD.Podemos criar uma entidade definindo uma nova classe e colocando @entity() antes.
        Para utilizarmos no nosso projeto devemos definir:"entities": ["src/entities/*.ts"]
        em nosso ormconfig.js
    ## Repositories
        Repository é como um manipulador de entidade, mas suas operações são limitadas a uma entidade concreta. Podemos utilizar um repositório de algum ORM ou criarmos o nosso repositório customizado, do qual geralmente é criado para uma unica entity e contem querys específicas.

    ## Service
        Tudo relacionado à criação de usuário, no nosso caso teremos as seguintes services:

        Cadastro de usuários,
        Cadastro de Tags,
        Listagem.

    ## Controller
        Responsável por repassar informações para o service após receber as informações do server.

    ###### 1) DB - Data Base = Banco de dados