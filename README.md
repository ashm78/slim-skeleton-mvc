# Slim 4 MVC Skeleton 

[![Codacy Badge](https://app.codacy.com/project/badge/Grade/62644bc058af464eb2cfcf564c3500d6)](https://www.codacy.com/gh/semhoun/slim-skeleton-mvc/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=semhoun/slim-skeleton-mvc&amp;utm_campaign=Badge_Grade) [![Latest Stable Version](https://poser.pugx.org/semhoun/slim-skeleton-mvc/v/stable)](https://packagist.org/packages/semhoun/slim-skeleton-mvc) [![Total Downloads](https://poser.pugx.org/semhoun/slim-skeleton-mvc/downloads)](https://packagist.org/packages/semhoun/slim-skeleton-mvc) [![Latest Unstable Version](https://poser.pugx.org/semhoun/slim-skeleton-mvc/v/unstable)](https://packagist.org/packages/semhoun/slim-skeleton-mvc) [![License](https://poser.pugx.org/semhoun/slim-skeleton-mvc/license)](https://packagist.org/packages/semhoun/slim-skeleton-mvc) [![Monthly Downloads](https://poser.pugx.org/semhoun/slim-skeleton-mvc/d/monthly)](https://packagist.org/packages/semhoun/slim-skeleton-mvc)

This is a simple web application skeleton project that uses the [Slim4 Framework](http://www.slimframework.com/):
* [PHP-DI](http://php-di.org/) as dependency injection container
* [Slim-Psr7](https://github.com/slimphp/Slim-Psr7) as PSR-7 implementation
* [Doctrine](https://github.com/doctrine/orm) as ORM
* [Twig](https://twig.symfony.com/) as template engine
* [Flash messages](https://github.com/slimphp/Slim-Flash)
* [Monolog](https://github.com/Seldaek/monolog)
* [Console](https://github.com/symfony/console)


## Prepare

1. Create your project:
```bash
composer create-project semhoun/slim-skeleton-mvc [your-app]
```
2. Create database: `./bin/console.php app:init-db`


## Run it:

1. `cd [your-app]`
2. `php -S 0.0.0.0:8888 -t public/`
3. Browse to http://localhost:8888


## Notice

- Set `var` folder permission to writable when deploy to production environment
- Default login/password is *admin*/*admin*
- To generate Doctrine entities:`./bin/console.php orm:convert-mapping --from-database annotation ./src/Entity`
    :warning: *Delete all entities before re-generate to update entities.*