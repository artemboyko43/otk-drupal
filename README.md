# OTK Drupal

OTK - One turn kill :). In this repo means minimum quantity of commands to install drupal and most popular environment.

### Requirements to install:
* [Docker-compose](https://docs.docker.com/compose/install) 

### Steps:

1. Up environment by on command, more information about ports, configuration in `docker-compose.yml`

    ```sh
    $ docker-compose up -d
    ```

2. Connect by ssh to container with php, also in container you have already installed `drush`, `composer`.

    ```sh
    $ docker-compose exec php sh
    ```

3. Install drupal8 by composer(**You should be connected to your php container**), I choose this template `drupal-composer/drupal-project`. But you can use other.

    ```sh
    $ composer create-project drupal-composer/drupal-project:8.x-dev /var/www/html/project --stability dev --no-dev --no-interaction
    ```

4. Open you project here http://drupal.docker.localhost:8000/

I use two good tools:
* [docker4drupal](https://github.com/Wodby/docker4drupal)
* [drupal composer template](https://github.com/drupal-composer/drupal-project)

