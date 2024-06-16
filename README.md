# Docker configuration file

### Contains the following settings:
* php;
    * optional extensions:
        * xdebug;
        * exif;
        * libjpeg62;
        * libfreetype6;
        * gd;
* nginx;
* databases:
  * mysql 8.0;
  * postgesql 15.0;
* adminer;
* meilisearch;

### Setup and launch:
1. Uncomment the required settings, change required settings.
2. Start building the docker container using `docker-compose up --build -d`