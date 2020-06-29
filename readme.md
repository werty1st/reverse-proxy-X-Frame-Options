# Intro

This repo demonstrates how to use a reverse proxy to upgrade the less flexible __X-Frame-Options__ header with a __Content-Security-Policy__ header.

## Setup

The local __/etc/hosts__ file needs to contain:

```bash
127.0.0.1       www.corp.com
127.0.0.1       form1.corp.com
```

## Docker

To start run:

```bash
docker-compose up
```

and navigate to: <http://www.corp.com:8080/>

## Caddy

To test the Caddy Version comment out the Apache section and remove the comments from the Caddy section in the docker-compose.yml
