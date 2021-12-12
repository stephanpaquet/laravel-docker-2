# laravel-docker-2

## Version
```
* Laravel Framework 8.75.0
* Composer version 2.1.14 2021-11-30 10:51:4
* PHP 8.1.0 (fpm-fcgi) (built: Nov 30 2021 07:26:25
* Node v16.13.1
* Npm 8.1.2
```

## Installation de base sans Laravel
```
git clone git@github.com:stephanpaquet/laravel-docker-2.git
cd laravel-docker-2.git
docker-compose up --build

http://localhost/
```

## Composer
```
docker-compose run --rm composer -V
docker-compose run --rm composer dump-autoload
```

## PHP
```
docker-compose run --rm php -v

```

## Installation d'un projet Laravel
```
rm -rf src/public/
docker-compose run --rm composer create-project laravel/laravel . 

// J'ai dû exécuter ces commandes pour corriger des erreurs Permission denied
rm -rf src/storage/logs/ &&  mkdir src/storage/logs
rm -rf src/storage/framework/sessions/ &&  mkdir src/storage/framework/sessions/
rm -rf src/storage/framework/views/ &&  mkdir src/storage/framework/views/

http://localhost/
```

## Node
```
docker-compose run --rm node -v
```

## NPM
```
docker-compose run --rm npm -v
docker-compose run --rm npm install
docker-compose run --rm npm run development
docker-compose run --rm npm run watch-poll

```

## Artisan
```
docker-compose run --rm artisan -V
```
