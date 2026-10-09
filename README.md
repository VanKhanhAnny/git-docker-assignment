# Git and Docker Starter Application

This repository contains a small Python web application packaged with Docker for easy deployment and used to practice Git branching and merging.

## Application

The application listens on port 8000 and returns a text response when accessed over HTTP.

## Verification

The running application should be verified using an HTTP request to port 8000.

## Usage

Build the image:

    docker build -t git-docker-app:test .

Run the container and map host port 8080 to container port 8000:

    docker run -d --name app-test -p 8080:8000 git-docker-app:test

Check the response:

    curl http://localhost:8080
