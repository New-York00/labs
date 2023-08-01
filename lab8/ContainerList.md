# Containers Lab - Docker

## Task 1: Container Management

1. List Containers:

* Command to list the Docker containers present in your environment
`docker ps -a`

2. Pull Latest Ubuntu Image:
* Command to pull the latest Ubuntu image from the Docker registry
`docker pull ubuntu:latest`

3. Run Container:
* Command to run a container using the Ubuntu image you just pulled
`docker run -d -i ubuntu`

4. Remove Image:
* Command to remove: 
`docker stop 1f3638ff4bbba155c03f4c734ab1c2516ab5066788a139404e184b0cf7d72934 &&  docker rm 1f3638ff4bbba155c03f4c734ab1c2516ab5066788a139404e184b0cf7d72934`