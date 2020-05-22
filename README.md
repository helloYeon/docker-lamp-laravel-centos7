# docker-lamp-laravel-centos7
This is a basic LAMP environment built using Docker Compose. It consists following.

- php7.3
- centos7
- apache2.4
- mysql8.0
- composer
- node js (Gulp)

## Constitution
```
docker-lamp-laravel-centos7/

├── docker
│   ├── db
│   │   └── my.cnf       # Sync to /etc/mysql/conf.d/my.cnf
│   └── web
│       ├── Dockerfile
│       ├── docker.conf  # Copy to /etc/httpd/conf.d/docker.conf
│       ├── php.ini      # Sync to /etc/php.ini
│       └── php73.conf   # Copy to /etc/httpd/conf.d/php73.conf
├── docker-compose.yml
├── logs
│   ├── access_log
│   ├── error_log
│   ├── mysql-error.log
│   ├── mysql-query.log
│   ├── mysql-slow.log
│   └── php-error.log
└── src

```


## Installation

1. clone this repository
  ```bash
  git clone git@github.com:yeon444/docker-lamp-laravel-centos7.git
  cd docker-lamp-laravel-centos7.git
  ```
1. run docker compose
```
docker-compose up -d --build

