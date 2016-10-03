# Docker HTTP Image
[![Docker Stars](https://img.shields.io/docker/stars/deployerpt/http.svg)](https://registry.hub.docker.com/u/deployerpt/http)
[![Docker Pulls](https://img.shields.io/docker/pulls/deployerpt/http.svg)](https://registry.hub.docker.com/u/deployerpt/http) [![](https://images.microbadger.com/badges/image/deployerpt/http.svg)](https://microbadger.com/images/deployerpt/http "Get your own image badge on microbadger.com")

This repository contains configuration files for building Docker image to create a simple HTTP server.

### Docker Compose

If you are using Docker Compose 

The following `docker-compose.yml` would sync the `code` folder width Apache `html` folder

```yaml
http:
  image: deployerpt/http
  ports:
    - "80:80"
  volumes:
    - ./code:/var/www/html
```
 