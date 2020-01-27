### Laravel Docker Environment

Environment PHP [php-fpm-laravel](https://github.com/Cyber-Duck/php-fpm-laravel)

## Specifications:

* PHP 7.4, 7.3, 7.2 / 7.1 / 7.0 / 5.6 / 5.4
* OpenSSL PHP Extension
* PDO PHP Extension
* SOAP PHP Extension
* Mbstring PHP Extension
* Tokenizer PHP Extension
* XML PHP Extension
* INTL PHP Extension
* PCNTL PHP Extension
* ZIP PHP Extension
* MCRYPT PHP Extension
* GD PHP Extension
* BCMath PHP Extension
* Imagick PHP Extension
* Memcached
* Composer
* Laravel Cron Job for the [task scheduling](https://laravel.com/docs/5.4/scheduling#introduction) setup
* PHP ini values for Laravel (see [`laravel.ini`](laravel.ini))
* xDebug (PHPStorm friendly, see [`xdebug.ini`](xdebug.ini)). Update env variable **XDEBUG** for **true** to enable remote xDebug in Dockerfile php folder.
* `t` alias created to run unit tests `vendor/bin/phpunit` with `docker-compose exec [service_name] t`
* `d` alias created to run Laravel Dusk browser tests `artisan dusk` with `docker-compose exec [service_name] d`
* `art` alias created to run the Laravel `artisan` command
* `fresh` alias created to migrate the database fresh and seed the seeders `artisan migrate:fresh --seed`
