# laravel-docker-2

## Version
```
* Composer version 2.1.14 2021-11-30 10:51:4
* PHP 8.1.0 (fpm-fcgi) (built: Nov 30 2021 07:26:25
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


## Installation 
```

docker-compose run --rm composer create-project laravel/laravel . 

```

