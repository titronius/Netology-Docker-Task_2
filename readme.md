# Task 2 for Docker-Netology

Сommands to build and start DockerImage, based on python:3.12-slim and django-app from /static:

```bash
# create image
docker build . --tag=django-crud:1.0

# check images
docker image ls

# run container based on custom image with port tunnelling
docker run -d -p 8000:8000 --name=django-crud django-crud:1.0

# check containers
docker ps

#go to localhost:8000
```