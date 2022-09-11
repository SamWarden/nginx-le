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

Launch docker containers

```bash
docker compose up
```
Wait until a message appears with the text `signal process started` and open your domain
