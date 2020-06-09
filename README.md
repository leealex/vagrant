# Development environment based on Debian 9

## Description
This is pre-packaged Vagrant box that provides you a development environment without requiring you to install PHP, a web server, and any other server software on your local machine. 

**Included software:**

- Debian 9
- Nginx 1.10.3
- MySQL 5.7
- PHP 7.4
  - Curl
  - Memcached
  - PHP-FPM
  - Xdebug v2.9.5
- Redis server
- Composer
- Git 2.11
- NodeJS 13.14
- Yarn 1.22.4

MySQL **root** user password: **root**

## Installation

**Prerequisites:**
- [VirtualBox](https://www.virtualbox.org)
- [Vagrant](https://www.vagrantup.com)


All you need to do is just clone this repo and run command inside a folder that contains **Vagrantfile**:

`vagrant up`

Your virtual machine will be available at http://10.10.10.100 (this can be changed in Vagrantfile)

## Upgrade

Before upgrading the box backup all your databases.

- vagrant box update
- vagrant destroy
- vagrant up
