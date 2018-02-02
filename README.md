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

- Run the docker container
```bash
docker-compose up -d
```



