# NGINX-LE - Nginx web and proxy with automatic let's encrypt

[Original repository](https://github.com/nginx-le/nginx-le/)

[Docker build](https://hub.docker.com/r/umputun/nginx-le/)

## Installation

`docker` and `git` required

Clone this repository

```bash
git clone https://github.com/SamWarden/nginx-le
cd nginx-le
```

Copy `.env.template` to `.env` and edit it for your domain and email

```bash
cp .env.template .env
```

Create an external `nginx-reverse-proxy` network. Use it to connect other containers and to proxy requests to them

```bash
docker network create nginx-reverse-proxy
```

Launch docker containers

```bash
docker compose up
```

Wait until a message appears with the text `signal process started` and open your domain
