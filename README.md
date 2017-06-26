## Tiny size redis-trib on top of alpine

This repository contains **Dockerfile** of [redis-trib](http://download.redis.io/redis-stable/src/redis-trib.rb) for [Docker](https://www.docker.com/)'s [automated build](https://hub.docker.com/r/sgrio/redis-trib/) published to the public [Docker Hub](https://hub.docker.com/).

### Docker Tags

`sgrio/redis-trib` provides only one single tagged image:

* `latest`

### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://hub.docker.com/r/sgrio/redis-trib/) from public [Docker Hub](https://hub.docker.com/): `docker pull sgrio/redis-trib`

### Usage

    docker run -it --rm sgrio/redis-trib \
	create --replicas 1 \
	127.0.0.1:7000 127.0.0.1:7001 127.0.0.1:7002 \
	127.0.0.1:7003 127.0.0.1:7004 127.0.0.1:7005
