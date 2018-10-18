# Docker image for a CentOS 6 Linux - Apache - PHP server

This docker container is created to supply a CentOS 6 image that is pre-configured to host a PHP website. No database software is included, but support for MySQL/MariaDB is included in the PHP installation.

## Usage

```console
docker create \
--name centos6_lap \
 -v </path/to/your/webroot>:/var/www/html \
 -p 80:80 \
 lgalastacia/centos6_lap

## Parameters

- --name : Give the docker container a logical name
- -v : map a local location to a location in the container
- -p : map network ports
