Test project

## Features

In the project directory, you can build and run a simple web app to count no. of visits on the webpage. It generates two containers 1. web server and 2. redis (to hold count)

## Build Docker image

### `docker build -t YOUR_DOCKER_ID/docker-redis .`

Docker builds an image from Dockerfile.

## Run container from image

Two ways:

1. Using docker run
### `docker run -p 4001:8081 YOUR_DOCKER_ID/docker-redis`
Creates a container running web server and redis in the same container

2. Using docker-compose 
### `docker-compose up`
Creates two containers, one for each - web server and redis

Access the web app from your browser https://localhost:4001 .Refresh to see the increase in number of visits.