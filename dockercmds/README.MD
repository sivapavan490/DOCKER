# Below cmd  will show the images exit in the server

     docker images

# below cmd will pull the images from dockerhub

     docker pull imagename:version

# To create container from image we use below cmd
    
     docker create imagename:version


# to saw running containers we use below cmd

    docker ps

# to  saw containers in all stages either it is running or stop

    docker ps -a

# to start the containers we use below cmd

    docker start container id 

# to stop the containers we use below cmd

    docker stop container id 

# to remove the containers we use below cmd

    docker rm container id 

# to remove images

    docker rmi imageid

# to remove all images in single cmd

    docker rmi `docker images -a -q`

# to run containers in background we use below cmd

    docker run -d imagename
# to run containers with port no we use below cmd

    docker run -d -p hostport:containerport imagename

#hostport: It will expose to the outside of environment. Through hostport only we can acess the container

# when we create docker container. Docker will give a randomname. if we want specific name to the container we use below cmd

    docker run -d -p hostport:containerport --name specificname imagename

# to login to the container we use below cmd

    docker exec -it containerid or name  bash

# if we want to inspect container we use below cmd

    docker inspect containerid

# how to build images from dockerfile locally

    docker build -t imagename:version .

# how to build images & push to dockerhub 

    docker build -t  username/imagename:version .

# how to build images & push to ECR NEXUS docker registry

    docker build -t ECR URL or NEXUS DOCKER REGISTRY URL/USERNAME/IMAGENAME:VERSION .

# 