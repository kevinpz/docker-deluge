# docker-deluge

## Overview
This project deploy a Deluge application to a Docker container.
The Docker base image is fedora.

## Usage
The Docker can be start with the following docker-compose file :
```
version: '2'

services:
  deluge:
    image: kevinpz/deluge
    restart: always
    volumes:
      - /home/profile/docker/deluge/config:/config
      - /home/profile/data:/data
    ports:
      - 8112:8112
```
