# Docker and Postgres


## Pull the image
    $ docker pull ricardoveronica/postgres-pgadmin:tagname

#### Before starting
Go to, docker-compose.yml and put your own data in services
For db:
* POSTGRES_DB
* POSTGRES_USER
* POSTGRES_PASSWORD
For pgadmin:
* PGADMIN_DEFAULT_EMAIL
* PGADMIN_DEFAULT_PASSWORD

### Run
    $ docker-compose up
    # For detached mode
    $ docker-compose up -d

### Start Postgres
    $ docker-compose exec db psql -U your_user your_db

### Go to your browser for start PGAdmin
0.0.0.0:16543

### Create a /code directory if you want to import .sql files from psql
    \i code/code/your.sql
