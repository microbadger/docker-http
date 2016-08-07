# Docker HTTP Image
[![Docker Stars](https://img.shields.io/docker/stars/deployerpt/http.svg)](https://registry.hub.docker.com/u/deployerpt/http)
[![Docker Pulls](https://img.shields.io/docker/pulls/deployerpt/http.svg)](https://registry.hub.docker.com/u/deployerpt/http)

This repository contains configuration files for building Docker image to create a simple HTTP server.

### Docker Compose

If you are using Docker Compose 

The following `docker-compose.yml` would sync the `code` folder width Apache `html` folder

```yaml
http:
  image: http
  ports:
    - "80:80"
  volumes:
    - ./code:/var/www/html
```
