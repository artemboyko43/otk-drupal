otk-drupal

Requirements: Docker, Docker-Compose.

docker exec PHP_CONTAINER_NAME composer create-project drupal-composer/drupal-project:8.x-dev /var/www/html --stability dev --no-interaction

PHP_CONTAINER_NAME - name of your container with php.