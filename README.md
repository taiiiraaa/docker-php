To run a PHP application in a docker container
---
### Install
[Docker](https://www.docker.com/products/docker)

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
$ php composer.phar update
```
### Run phpunit
```bash
$ ./bin/phpunit [--debug]
```
