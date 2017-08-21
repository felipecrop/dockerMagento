# dockerMagento

## What's Inside
* [Nginx](http://nginx.org/)
* [PHP-FPM](http://php-fpm.org/)
* [Mysql](http://www.mysql.com/)
* [Redis](http://redis.io/)


## What's Commented
* [MongoDB](http://www.mongodb.org/)
* [Memcached](http://memcached.org/)
* [Elasticsearch](http://www.elasticsearch.org/)
* [RabbitMQ](https://www.rabbitmq.com/)
* [Solr](http://lucene.apache.org/solr/)
* [Gearman](http://gearman.org/)


## Requirements
* [Docker Engine](https://docs.docker.com/installation/)
* [Docker Compose](https://docs.docker.com/compose/)
* [Docker Machine](https://docs.docker.com/machine/) (Mac and Windows only)

## Running
Set up a Docker Machine and then run in background (inside you docker path):
```sh
$ docker-compose up
```

## Xdebug

It happened on an Ubuntu machine not to run Xdebug, it was necessary to execute a command to release the port:

sudo iptables -I INPUT -p tcp -m tcp --dport 9000 -j ACCEPT
