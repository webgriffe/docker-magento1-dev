Magento 1.x Development Docker Container
========================================

Dockerized environment for Magento 1.x development with PHP and Apache as web server.

Features
--------

* Based on [webgriffe/php-apache-base](https://hub.docker.com/r/webgriffe/php-apache-base/) Docker image. Look at its README for more info.
* [n98-magerun.phar](https://github.com/netz98/n98-magerun) installed globally at `/usr/local/bin/composer`
* MySQL CLI client installed because is required by n98-magerun db commands
* [Memcached](http://php.net/manual/en/book.memcached.php) PHP extension installed and enabled (useful for Magento cache & session storage)

Usage
-----

Standalone usage example with host's current working directory as document root:

	$ docker run -p 80:80 -v $(pwd):/var/www/html webgriffe/magento1-dev

Credits
-------

[Webgriffe®](http://www.webgriffe.com/)




