---
layout: post
title: "Deploy Clouflare DDNS on Docker"
date: 2022-01-12 19:00:00 +0800
categories: [Tutorial, Server, Docker]
---


Docker Compose to install Cloudflare Dynamic Dns on your server

```
version: '2'
services:
  cloudflare-ddns:
    image: oznu/cloudflare-ddns:latest
    restart: always
    environment:
      - API_KEY=**************************
      - ZONE=example.com
      - PROXIED=true
      - PUID=1000
      - PGID=100

```