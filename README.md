# Docker Compose Nginx Proxy
This is a simple example of a Docker setup using Docker Compose to create an Nginx Proxy with SSL support.

This setup uses the default nginx Docker repository along with:
- [https://github.com/jwilder/docker-gen](https://github.com/jwilder/docker-gen)
- [https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion)

There are some slight adjustments to the Nginx configurations to allow for long headers. This is because a tool we commonly use includes long cache tag headers which cannot be configured right now. Also there are a couple of recommended speed optimisations. This is a very small repository so please just take a look around at the few files here and feel free to clone this repository if you find it helpful.