# java-web-app-docker

Deploying Java web application in one server 

steps involved in Jenkins file
* changing source code into war file using Maven build tool
* Making war file as Docker image by building Dockerfile
* Push the Docker image into DockerHub
* Running Docker container in deployment server

For this, we need to have 2 aws servers.
one is for Jenkins and another is for deploying application

In Jenkins server, we need to install Java and Jenkins

To work Docker commands in Jenkins console, we need to add Jenkins user in Docker group in command line using
* usermod -aG docker jenkins

In Deployment server, we need to download docker 

we need to add ubuntu user in docker group to login server and execute docker container commands

* usermod -aG docker ubuntu
