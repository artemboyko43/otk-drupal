# OTK Drupal

OTK - One turn kill :). In this repo means minimum quantity of commands to install drupal and most popular environment.

### Steps:

```sh
$ docker-compose up -d
$ docker exec PHP_CONTAINER_NAME composer create-project drupal-composer/drupal-project:8.x-dev /var/www/html --stability dev --no-interaction
```

I use two good tools:
* [docker4drupal](https://github.com/Wodby/docker4drupal)
* [drupal composer template](https://github.com/drupal-composer/drupal-project)