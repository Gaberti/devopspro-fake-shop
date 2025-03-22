# Fake Shop


## Variável de Ambiente
DB_HOST	=> Host do banco de dados PostgreSQL.

DB_USER => Nome do usuário do banco de dados PostgreSQL.

DB_PASSWORD	=> Senha do usuário do banco de dados PostgreSQL.

DB_NAME	=>	Nome do banco de dados PostgreSQL.

DB_PORT	=>	Porta de conexão com o banco de dados PostgreSQL.


## Execução Pipeline - Github Actions

1. Fazer o commit e push para a branch main
2. Acompanhar execução de jobs
    a. Job CI
        i. Com criação da imagem
        ii. Com deploy no docker hub
    b. Job CD
        i. Get do Config do cluster kubernetes na DigitalOcean (secret)
        ii. Com deploy na pipeline do DigitalOcean
    c. Acompanhar o IP público correspondente ao cluster