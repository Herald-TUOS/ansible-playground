A dockerized container for learning ansible

# Prerequisites:

- Docker
- Docker Compose

# Playground nodes

-  A control node container running python slim official image
-  One managed host: Alpine linux

# Config

Run `ssh-keygen -t rsa -N "" -f secrets/id_rsa` generate a SSH key pair in `./secrets`. 

This will be used to connect to managed hosts by the control node.

# Setup using docker compose

### Setup
- Run `docker-compose up -d` to start containers

### Run ansible
- `docker-compose exec controlnode bash`
- `ansible --version`

### Cleanup
- `docker-compose down`


This repo takes inspiration from [here](https://github.com/abdennour/ansible-lab-environment-in-containers).