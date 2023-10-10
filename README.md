# Laravel 9.x - Quick Start (Laravel 9.x + Docker)

## Launch Laravel

Clone Repository

```sh
git clone https://github.com/devfullcycle/FC3-admin-catalogo-de-videos-php.git laravel9
```

```sh
cd laravel9/
```

Remove versioning (optional)

```sh
rm -rf .git/
```

Create the .env file

```sh
cp .env.example .env
```

Update the .env file environment variables

```dosini
APP_NAME="Admin Video Catalog"
APP_URL=http://localhost:8000

DB_CONNECTION=mysql
DB_HOST=db
DB_PORT=3306
DB_DATABASE=code_micro_videos
DB_USERNAME=root
DB_PASSWORD=root

CACHE_DRIVER=redis
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
```

Launch project containers

```sh
docker-compose up -d
```

Access the app container

```sh
docker-compose exec app bash
```

Install project dependencies

```sh
composer install
```

Generate the Laravel project key

```sh
php artisan key:generate
```

Access the project
[http://localhost:8000](http://localhost:8000)
