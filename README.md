# Docker Custom Website

This project demonstrates how to build and run a custom Docker image using Nginx.

## Project Overview

In this project I created a simple HTML webpage and deployed it inside a Docker container using Nginx.

This helped me understand how Docker images and containers work.

## Technologies Used

- Docker
- Nginx
- Linux
- HTML

## Project Steps

1. Created a simple HTML webpage
2. Wrote a Dockerfile using Nginx as the base image
3. Copied the HTML file into the container
4. Built a custom Docker image
5. Ran the container and exposed it on localhost

## Dockerfile
FROM nginx
COPY index.html /usr/share/nginx/html/index.html

## Build Image
docker build -t vignesh-nginx .

## Run Container
docker run -d -p 8081:80 vignesh-nginx

## Access Website
http://localhost:8081

## Learning Outcome
- Understanding Docker images
- Building custom Docker images
- Running containerized web servers
- Port mapping between container and host
