# viktoriya666_microservices
viktoriya666 microservices repository

HW Docker -2 (#15)

- Created a new branch Docker-2
- Connecting TravisCI
- The output of the docker images -a command has been added to docker-monolith \ docker-1.log

HW Docker -3 (#16)

The application consists of:
post-py - post writing service
comment - the service responsible for writing comments
ui - a web interface that works with other services

Files created:
post-py / Dockerfile
comment / Dockerfile
ui / Dockerfile

- I downloaded the latest version of MongoDB image
- Collected images
- Created a network for the application
- Launched containers on this network
- Added network aliases to containers

CHECK:
http://35.240.126.98:9292

HW Docker -4 (#17)

- worked with docker-compose;
- added docker-compose.yml file;
- worked with docker networks;
- described the application in docker-compose.

!!! При запуске проекта с помощью docker-compose, все сущности создаются с префиксом равным каталогу, где лежит docker-compose.yml. Это считается базовым именем проекта. Поменять его можно, указав в .env параметр: COMPOSE_PROJECT_NAME=<new_name>

RUN:

- go to the src directory
- rename the file .env.example to .env
run the command:
- docker-compose -f docker-compose.yml build
- docker-compose -f docker-compose.yml up -d

CHECK:
- go to link http://docker_host_ip:зport


HW Gitlab-ci  (#18)

В процессе сделано:

- deployed gitlab-ce to Google Cloud Platform;
- configured CI/CD for Reddit

HW Monitoring-1  (#19)

- Created a Docker host in GCE and set up a local environment
- Set up Prometheus
- Added to the configuration node-exporter
- Added images to the docker hub

RUN:
link to images DockerHub
https://hub.docker.com/repository/docker/viktoriya666


HW Monitoring-2  (#20)

- Connected container monitoring using cAdvisor
- Added visualization using Grafana
- Imported a dashboard for monitoring Docker
- We connected an alert manager with notifications in Slack channel #viktoriya_volferts

RUN:
link to images DockerHub
https://hub.docker.com/repository/docker/viktoriya666