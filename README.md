Atualize as variáveis de ambiente do arquivo .env
```dosini
APP_NAME=Lara_Postgres
APP_URL=http://localhost:8000

DB_CONNECTION=psql
DB_HOST=pgsql
DB_PORT=5432
DB_DATABASE=nome_que_desejar_db
DB_USERNAME=postgres
DB_PASSWORD=postgres

CACHE_DRIVER=redis
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
```


Suba os containers do projeto
```sh
docker-compose up -d
```


Acessar o container
```sh
docker-compose exec app bash
```


Instalar as dependências do projeto
```sh
composer install
```


Gerar a key do projeto Laravel
```sh
php artisan key:generate
```


Acesse o projeto
[http://localhost:8180](http://localhost:8180)