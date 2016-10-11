# MariaDB Container for Dogs

Create a _MariaDB_ service with a default database that we can use for developments at Dogstudio : 

* User: `root`
* Passsword: `docker`
* Dataabse: `docker_dev`

> This Container is used only for developments !

## In `docker-compose.yml`

    services:
      database:
        image: dogstudio/mariadb
        ports:
          - "3306:3306"

Because we use _"Docker for Mac"_, the database is available in `localhost:3306` with application like _"Sequel Pro"_.
