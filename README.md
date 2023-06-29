# php-docker

docker build -t hello-php
docker images
docker run -p 3000:80 hello-php
docker run -p 3000:80 -d hello-php
docker run -p 5000:80 -d -v $(pwd)/src:/var/www/html/ hello-php

# docker build -t hello-php:tag
docker build -t hello-php:1.0
docker run -p 4000:80 -d --name myserver hello-php:1.0
