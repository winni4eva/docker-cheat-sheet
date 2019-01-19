# docker-cheat-sheet

## Installation
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04

## Commands
- docker run hello-world => run image hello-world
- docker ps => view only active containers
- docker ps -a => view all containers
- docker ps -l => lastest container created
- NB: You can refer to docker containers with names and id's. Container name is auto generated if you dont specify one
- docker run --name my-hello hello-world => specify a custom name for our docker container [you can add --rm flag to delete container after exit]
- docker search ubuntu => searches for ubuntu images on docker hub
- docker pull ubuntu => to download official ubuntu image unto your machine
- docker images => view list of downloaded images
- docker run -it ubuntu => the it flag enables an interactive shell into the container
- exit => to exit a containers interactive shell
- docker start d9b100f2f636 => start a stopped container with id or name
- docker stop my-ubuntu => stop container with id or name
- docker rm my-ubuntu => remove a container from your system
- docker commit -m "What you did to the image" -a "Author Name" container_id repository/new_image_nam => commit changes to a new docker image
- NB: You can also build images from a docker file, which lets you automate the installation of software

## Pushing Images To The Docker Repository
### After creating a custom image from a default one you would need a way to share it with your friends
- Create an account on docker hub
- Docker hub is a public repo for images, however you can setup a private docker registry for your images