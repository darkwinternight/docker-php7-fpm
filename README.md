# PHP 7.1 FPM

All-purpose PHP-FPM 7.1 Docker image. Find it on [Dockerhub](https://hub.docker.com/r/winternight/php7-fpm/builds/).

`$ docker pull winternight/php7-fpm:7.1`

## Description

This is a docker image for an all-purpose PHP-FPM (PHP Version 7.1) container.  It is based on the `7.1-alpine` tag of the [official PHP Docker image](https://hub.docker.com/_/php/). [Patch version](http://semver.org) upgrades are thus done automatically on build (e.g. `7.0.11` to `7.0.12`) but for minor version upgrades (e.g. `7.1.x` to `7.2.x`), a new Dockerfile should be created and tagged appropriately.

## Extensions

The installed extensions are enough for [Laravel 5 projects](https://laravel.com) as long as the project is using MySQL. If you need other database drivers/extensions, please fork this image.

This is the full list of preinstalled PHP extensions in this image:

- `ctype`
- `curl`
- `dom`
- `gd`
- `hash`
- `iconv`
- `intl`
- `json`
- `mbstring`
- `mcrypt`
- `mysqli`
- `opcache`
- `pdo`
- `pdo_mysql`
- `phar`
- `posix`
- `session`
- `simplexml`
- `sockets`
- `tokenizer`
- `xml`
- `xmlrpc`
- `xmlwriter`
- `zip`


## Building

In order to build this image yourself, simply run the following command:

`$ docker build -t winternight/php7-fpm:7.1 .`