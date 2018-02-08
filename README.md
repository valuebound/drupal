Drupal Base
============

[![Latest Stable Version](https://poser.pugx.org/valuebound/drupal/v/stable)](https://packagist.org/packages/valuebound/drupal) [![License](https://poser.pugx.org/valuebound/drupal/license)](https://packagist.org/packages/valuebound/drupal) [![composer.lock](https://poser.pugx.org/valuebound/drupal/composerlock)](https://packagist.org/packages/valuebound/drupal)

A composer workflow based Drupal repository to be used as a base for Drupal projets. It is bundled with standard tools for development like Drush, Drupal console, PHPUnit & PHPCS. A set of highly popular & necessary contributed modules is also included to serve a starting for any Drupal 8 project.

***Follow the below steps to create a new projects***

### Pre-Requisites
-----------
 - **Docker** - https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-16-04
 - **Docker Compose** - https://www.digitalocean.com/community/tutorials/how-to-install-docker-compose-on-ubuntu-16-04
 

### Usage
---------
- Using composer get the repository
```bash
composer create-project valuebound/drupal drupal
```
- Copy exmaple.docker-compose.yml to docker-compose.yml.
- Copy example.env to .env
- Update the .env file to suit set your variables for the container
- Update docker to use [Traefik reverse proxy](https://www.digitalocean.com/community/tutorials/how-to-use-traefik-as-a-reverse-proxy-for-docker-containers-on-ubuntu-16-04) (if you know what you are doing then only edit this file, else leave as it is).
- Run the docker container
```bash
docker-compose up -d
```

### Additional useful tips
- To view the containers `docker-compose ps`
- To stop all the container `docker-compose stop`
- To restart the containers `docker-compose restart`
- To remove the containers `docker-compose rm`

### Drupal tools usage
- #### Drush
The repository ships with `Drush` version `9.0.0`. Ideally if you have Drush installed in your system you can directly use it like in any other project. If not use `./vendor/bin/drush [command]`.

** N.B - If the above doesn't work, use the docker-compose to run drush**
`docker-compose exec web drush [command]`

- #### Drupal Console
`./vendor/bin/console [command]`

- #### PHP Codesniffer
`./vendor/bin/phpcs [command]` 



