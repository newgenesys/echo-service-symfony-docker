## Description

This is a complete stack for running Symfony into a Docker container using docker-compose tool for ech-service app to resident automatically.

It is composed by 4 containers:

- `nginx`, acting as the webserver.
- `php`, the PHP-FPM container with the 8.1 version of PHP.
- `db` which is the MySQL database container with a **MySQL 8.0** image.
- `app` which is the ech-service symfony app to be setup

Build the Docker images:

    docker compose build --no-cache --pull

Start the project!

    docker compose up -d

Browse `https://localhost`, your Docker configuration is ready!
