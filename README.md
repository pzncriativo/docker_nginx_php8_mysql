
### Setup Docker Para WEB - NGINX + PHP8 + MYSQL

### Passo a passo
Clone Repositório
```sh
git clone https://github.com/pzncriativo/setup_docker_pzn_web_app_v1.git
```

```sh
cd setup_docker_pzn_web_app_v1/
```

Crie o Arquivo .env
```sh
vim .env
```

Atualize as variáveis de ambiente do arquivo .env
```dosini
APP_NAME=pzn
APP_URL=http://localhost

DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=nome_que_desejar_db
DB_USERNAME=nome_usuario
DB_PASSWORD=senha_aqui

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

Acessar o projeto
[http://localhost](http://localhost)
