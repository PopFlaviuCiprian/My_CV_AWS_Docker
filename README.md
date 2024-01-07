
# Workflow
In this mini project I build several Docker containers that contains a static portfolio website written in HTML-CSS in Visual Studio Code.

# Requirements

- Docker
- Visual Studio Code
- Flask
- Filezilla
- SuperPuTTy


# Install Docker
```
sudo apt update
sudo apt install docker.io
```
# Install Visual Studio Code

https://code.visualstudio.com/downloadvi


# Install Filezilla

https://filezilla-project.org/

# Install SuperPuTTy 

https://www.puttygen.com/superputty

### Building the project

The structure of the project will be as follow:

app.py        - a file that contains a Flask web framework for our website

Dockerfile    - this file contains the instructions for bulding our docker image

requirements  - this file contains our dependencies for this project which is Flask

index.html    - our static website written in html-css 

### Building the image and containers

```
docker build -t my_docker_cv .  (build the image)

docker run --name my_portfolio -d -p 5000:5000 my_docker_cv (running a container named my_portfolio that can be accessed on http://localhost:5000)

docker ps (this command will list the running containers)

```