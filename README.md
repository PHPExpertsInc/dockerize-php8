# Dockerize PHP v8.0!

A utility for rapidly deploying PHP v8.0 for testing against your existing projects.

Includes: 
 * PHP v8.0 beta 4 
 * Extra extensions:
   * bcmath
   * curl
   * gd
   * gmp
   * iconv
   * mbstring
   * mysqlnd
   * pdo_mysql
   * pdo_pgsql
   * xml
   * xmlreader
   * xmlwriter
   * zip

It is based off of [**phpexperts/dockerize**](https://github.com/phpexpertsinc/dockerize-php).

# Installation

    composer require --dev phpexperts/dockerize-php8
    
    # If you want nginx + PHP-FPM and/or mysql/mariadb/postgres/redis:
    php vendor/phpexperts/dockerize-php8/install.php

### Installation Video

https://youtu.be/xZxaJcsbrWU

### Configure your PATH

Ensure that your profile PATH includes `./vendor/bin` and that it takes priority over any other directory that may include a php executable:

    PATH=./vendor/bin:$PATH

# Running

Run as normal.

If you want to revert back to your built-in version of PHP, do this:

    export PHP_VERSION=native

It will then use your system-level PHP.

You can also set `PHP_VERSION` to any other major PHP version (5.6-8.0).
See [**phpexperts/dockerize-php**](https://github.com/phpexpertsinc/dockerize-php) for more.

# About PHP Experts, Inc.

[PHP Experts, Inc.](https://www.phpexperts.pro/), is my consultation company. It's a small company of a half dozen 
highly skilled Full Stack PHP devs, including myself, whom I place at 1099 positions at other corporations. We fill both 
long-term positions and, for crazy devs like me, short-term. If you ever wanted to work on a different project/company 
every few months or even weeks, anywhere in the continental U.S., Europe, or South East Asia, it's fantastic.  

Since 2015, I have set up branches in Las Vegas, Houston, the UK, Dublin, Costa Rica, Colombia, India, and the Philippines. 
If someone has a work auth in any of those places, we can place you almost anywhere you want. I travel 50% of the time 
out of choice. All over the world.

Plus, no taxes if you spend 6+ months (or a year, if you're American) out of your country. 
