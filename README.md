# poc-unpkg-docker-server

Proof of concept of an unpkg-server in a docker environment.  
The Dockerfile is based upon [this](https://nodejs.org/de/docs/guides/nodejs-docker-webapp/) official node.js guide.

## Commands

- `docker build -t denniska/poc-unpkg-docker-server .`
    - Builds the container
- `docker run -p 49160:8080 -d denniska/poc-unpkg-docker-server`
    - Runs the container
    - Maps port 8080 inside the container to port 49160 on the host
- `docker ps`
    - Get the container ID
- `docker logs <container id>`
    - Print app output
