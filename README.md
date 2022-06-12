# docker-apache2-php-mariadb-composer
Docker running Apache2, PHP, Composer, MariaDB &amp; PHPMyAdmin



> Although I prefer NGINX, it is sometimes necessary to use Apache as well. That's why I add docker-compose here, which I use here and there.

---


.env file structure

Variable name | Variable default value | Description
--- | --- | ---
APP_PORT | 8000 | port for Apache - http://localhost:APP_PORT
PHPMYADMIN_PORT | 8080 | port for PHPMyAdmin
APP_DIR | ./app | directory containing the website
PHP_VERSION | 7.4 | PHP Version - https://hub.docker.com/_/php?tab=tags
MARIADB_DATA_DIR | ./.docker/mysql/data | MariaDB data storage directory
MARIADB_DATABASE | app | Database name
MARIADB_ROOT_PASSWORD | t00r | The root password
MARIADB_USER | app | Database user name
MARIADB_PASSWORD | t00r | Database user password


<hr>

.env file example
```APP_PORT=8001
PHPMYADMIN_PORT=8081

APP_DIR=./app
MARIADB_DATA_DIR=./.docker/mysql/data
PHP_VERSION=7.4

MARIADB_DATABASE=app
MARIADB_ROOT_PASSWORD=t00r
MARIADB_USER=app
MARIADB_PASSWORD=t00r
```
