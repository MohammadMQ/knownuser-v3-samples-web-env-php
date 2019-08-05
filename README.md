# knownuser-v3-samples-web-env-php
Create docker image that setup apache web development environment for knownuser-v3-samples (php 5 or 7), so that the site kan be browsed in a browser (BuyTickets.php being the first page)

This repo will only contain following files:
- docker-compose.yml
- docker-php7.dockerfile

These files are to be placed in the following folder of repository: **knownuser-v3-samples**: 
knownuser-v3-samples/php/sample/ 

(NB: If another php version needs to be supported like PHP 5, then just add another docker file and name it e.g. docker-php5.dockerfile and let it pull a docker php5 image e.g. **php:5.3-apache**)

Open the docker-compose.yml file and point towards the relevant docker-tests-php?.dockerfile, hereafter run the following docker commands:

docker-compose build
docker-compose up

Open a browser and to to: 127.0.0.1:8000

## Conclusion
Above docker commands will setup up web development environment, so knownuser can be browsed in browser from the url 127.0.0.1:8000

