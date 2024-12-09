# D O C K E R S

### How to install:
``` bash
sudo apt install docker.io
```

##### How to create image using Dockerfile:
``` bash
docker build -t repo-image .
```
##### How to run container using image
``` bash
docker run -d --name c1 -p 8001:8001 repo-image tail -f /dev/null
```

##### Build using docker-compose.yml
``` bash
docker-compose up -d --build
```

##### Access Shell inside the container
``` bash
docker exec -it c1 /bin/bash
```
##### Stop Container
``` bash
docker stop name
```
##### Delete Container
``` bash
docker rm -f name
```
##### Delete Image
``` bash
docker rmi -f name
```
##### List images
``` bash
docker images
```
