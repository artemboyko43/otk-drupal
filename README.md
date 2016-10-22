otk-drupal

Requirements: Docker, Docker-Compose.

Steps for installing.

1. docker-compose up -d

2. docker exec PHP_CONTAINER_NAME composer create-project drupal-composer/drupal-project:8.x-dev /var/www/html --stability dev --no-interaction

PHP_CONTAINER_NAME - name of your container with php.

Thanx for:
https://github.com/Wodby/docker4drupal 
https://github.com/drupal-composer/drupal-project
