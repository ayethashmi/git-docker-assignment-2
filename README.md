# Git and Docker Starter Application

This repository contains a small Python web application used to practice Git, GitHub, and Docker workflows.

## Application

The application listens on port 8000 and returns a text response when accessed over HTTP.

## Verification

The running application should be verified using an HTTP request to port 8000.

## Usage Instructions

### Build the Docker Image

Build the application image using:

docker build -t git-docker-app:test .

### Run the Application

Start the application container:

docker run -d --name app-test -p 8080:8000 git-docker-app:test

The application runs on port 8000 inside the container and is accessible through port 8080 on the host.

### Test the Application

Verify that the application responds successfully:

curl http://localhost:8080

Expected response:

Advanced Git Docker App - Version 2
Status: healthy - aayet
Environment: production

### View Container Logs

docker logs app-test

### Stop and Remove the Container

docker stop app-test
docker rm app-test
