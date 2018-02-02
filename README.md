Drupal Base
============

A composer workflow based Drupal repository to be used as a base for Drupal projets. It is bundled with standard tools for development like Drush, Drupal console, PHPUnit & PHPCS. A set of highly popular & necessary contributed modules is also included to serve a starting for any Drupal 8 project.

***Follow the below steps to create a new projects***

### Pre-Requisites
-----------
 - **Docker** - https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-16-04

 - **Docker Compose** - https://www.digitalocean.com/community/tutorials/how-to-install-docker-compose-on-ubuntu-16-04
 

### Usage
---------
- Clone the repository

```bash
git clone git@bitbucket.org:malabya/drupal.git PROJECTNAME
```

- From the repository, install the composer dependencies

```bash
cd PROJECTNAME
composer install
```

- Run the docker container
```bash
docker-compose up -d
```



