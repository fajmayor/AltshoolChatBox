# Deployment of AltschoolChatBot (A PHP WebApp) to Kubernetes Cluster
This document outlines the deployment process for AltSchool's ChatBot application, which is built using PHP, MySQL, and jQuery, onto a Kubernetes cluster. Following these steps will ensure a smooth deployment of the application.

# Installing The Application
```
From Database Folder Import chat.sql into your database
Run Your Server
Type localhost/chatbot/chatbot.php on your Browser
```

# DevOps Steps
## Containerize the ChatBot Application
- Dockerize the PHP, MySQL, and jQuery application components by choosing PHP:7.2-apache base image
- Best docker practice was followed
## Build Dockerfile and Push to Docker hub
- Build Dockerfile to image
- Push the Docker image to a Docker registry accessible by the Kubernetes cluster.
## Create Kubernetes Deployment Manifests
- Kubernetes Deployment manifest files for each component are created; `mysql-deployment.yaml`, `mysql-pv.yaml`, and `php-deployment.yaml`
- Environment variables, volumes, and other required settings are configured in the manifest files
- I ensured proper resource requests and limits were set for each container
## Prepare Kubernetes Environment


## Deploy in Kubernetes






