# Connect with Nginx

## Prerequisites

### Mac

* [docker](https://docs.docker.com/installation/mac)
* [docker compose](https://docs.docker.com/compose/install)

### Ubuntu

Docker

    wget -qO- https://get.docker.com/ | sh
    sudo usermod -aG docker <your unix user>
    logout

Docker-compose

    sudo -i
    curl -L https://github.com/docker/compose/releases/download/1.1.0/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
    chmod +x /usr/local/bin/docker-compose
    curl -L https://raw.githubusercontent.com/docker/compose/1.1.0/contrib/completion/bash/docker-compose > /etc/bash_completion.d/docker-compose

## Setup

    sudo sh -c "echo '127.0.0.1 laptop-connect.anvil.io' >> /etc/hosts"

on mac replace 127.0.0.1 with the output of `boot2docker ip`

## Run
    ./run                              # run on https://laptop-connect.anvil.io
    open https://laptop-connect.anvil.io/.well-known/openid-configuration

## Misc

NODE_HOST=connect.anvil.io ./run   # run on https://connec.anvil.io

Generating SSL Certificate: https://www.digitalocean.com/community/tutorials/how-to-create-an-ssl-certificate-on-nginx-for-ubuntu-14-04
Architecture: http://anandmanisankar.com/posts/docker-container-nginx-node-redis-example/

### Docker commands

    docker-compose ps
    docker-compose run --service-ports connect sh   # run command with ports

