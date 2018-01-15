## This is a quick setup of Python3 and Postgresql using docker-compose

`requirements.txt`

This file is used to install additional software besides Python parent image

## Useful commands

`docker-compose up`

Start containers

`docker-compose up -d`

Start containers in detached mode (as a daemon)

`docker-compose up -d --build`

Rebuild the containers in case of adding new libraries, or modifying docker-compose.yaml

`docker-compose run web django-admin.py startproject composeexample .`

Example of how to run a command inside a container. In this case, we run the command startproject of 
django-admin.py executable in the web container. In general, if we want to run django commands:

`docker-compose run web ...`

Where ... is the command we want to run inside that container.

`docker ps`

List running containers

`docker-compose down`

Stops running containers


Built with

https://docs.docker.com/compose/django

Here is the tutorial with how to deploy to a nginx.

https://www.capside.com/labs/deploying-full-django-stack-with-docker-compose/