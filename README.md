Run a PHP application in a docker container
---
### Install
[Docker](https://www.docker.com/products/docker)

### Directory
Go to the directory where this repository was cloned.

E.g:
```bash
$ cd /var/www/docker-php
```

### Build Container
```bash
$ docker-compose build
```
### Start Container
```bash
$ docker-compose up [-d]
```
-d to run in detached mode

### Run bash in container
```bash
$ docker exec -it containername_php_1 /bin/bash
```

### Run composer
```bash
$ cd app
$ php composer.phar update
```

### Run phpunit
```bash
$ ./bin/phpunit [--debug]
```

### HTTP access
```
http://localhost:8080/
```

### Mysql access
```
127.0.0.1:32776
root:root
```

### Packages
- php:7.0-fpm. To change PHP version, update docker/php/Dockerfile.
- nginx:stable. To change Nginx version, update docker/nginx/Dockerfile.
- mysql:5.7. To change Mysql version, update docker-compose.yml
