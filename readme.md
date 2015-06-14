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

## Run

    ./run
    
## Misc

Generating SSL Certificate: https://www.digitalocean.com/community/tutorials/how-to-create-an-ssl-certificate-on-nginx-for-ubuntu-14-04
Architecture: http://anandmanisankar.com/posts/docker-container-nginx-node-redis-example/
