# Project Documentation

## Overview

This project involves the creation, configuration, and deployment of multiple Docker applications, using Nginx as a reverse proxy to manage traffic and Kubernetes for container orchestration. The applications include Plik, Wiki.js, OneTimeSecret, and EJBCA-CE.

## Project Structure

### Docker Applications

1. **Plik**: A file-sharing service.
2. **Wiki.js**: A wiki-based documentation platform.
3. **OneTimeSecret**: A service for securely sharing secrets.
4. **EJBCA-CE**: An open-source certificate authority (CA) implementation.

### Nginx Configuration as Reverse Proxy

Nginx is configured as a reverse proxy to redirect traffic from various applications to their respective internal ports. This allows all applications to be accessible through a single entry point.

### Kubernetes for Orchestration

Kubernetes is used to manage the deployment, scalability, and operation of the containerized applications. This includes creating deployments, services, and using restart policies to ensure high availability.

## Steps Performed

### 1. Creating Docker Containers

Each application was containerized using Docker. This process included writing Dockerfiles and building the Docker images.

Example command to build and tag a Docker image:

```sh
docker build -t username/repository:tag .
docker push username/repository:tag
