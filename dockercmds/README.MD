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