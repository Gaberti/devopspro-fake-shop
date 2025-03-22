# Fake Shop


## Variável de Ambiente
DB_HOST	=> Host do banco de dados PostgreSQL.

DB_USER => Nome do usuário do banco de dados PostgreSQL.

DB_PASSWORD	=> Senha do usuário do banco de dados PostgreSQL.

DB_NAME	=>	Nome do banco de dados PostgreSQL.

DB_PORT	=>	Porta de conexão com o banco de dados PostgreSQL.


## Execução Pipeline - Github Actions

- Fazer o commit e push para a branch main
- Acompanhar execução de jobs
    - Job CI
        - Com criação da imagem
        - Com deploy no docker hub
    - Job CD
        - Get do Config do cluster kubernetes na DigitalOcean (secret)
        - Com deploy na pipeline do DigitalOcean
    - Acompanhar o IP público correspondente ao cluster