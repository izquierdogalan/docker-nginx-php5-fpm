docker-nginx-php5-fpm
==================

This is the base image with Ubuntu, Nginx and PHP FPM. Docker repository available here [izquierdogalan/docker-nginx-php5-fpm](https://registry.hub.docker.com/u/izquierdogalan/docker-nginx-php5-fpm/).

**Installed Ubuntu version:**
- 15.04

**Installed software:**
- [Nginx 1.4.6](http://nginx.org/)
- [PHP FPM 5.6.x](http://www.php.net)

**Installed tools:**
- nano
- curl
- git

**Installed PHP modules:**
- cli
- intl
- mcrypt
- apcu
- gd
- curl

**Build**

	docker build -t "izquierdogalan/nginx-php-fpm" .

**Run**

	docker run -t -i -p 8080:80 -d "izquierdogalan/nginx-php-fpm" /bin/bash

**Launch**

	http://localhost:8080/

Note, if you have used the boot2docker virtual machine, you'll need to get the IP of the virtual host instead of using localhost. You can do this by running the following command `boot2docker ip`.
