# Docker-server-project
In this project, I ran a container that do not immediatiely exit after running the entry point commands.

STEP 1 - Inspect the server.Docker file that copies ./server.bash / intead of the entry point 
Run vim sever.Dockerfile 

STEP 2 - Build, start and tag container 
Run docker build --file server.Dockerfile --tag "name of image"

STEP 3 - Create container from tagged image without attaching the terminal 
Run docker run -d "name of image"

STEP 4 - Confirm containing is running 
run docker ps 

STEP 4 - Run additional command from the container 
run docker exec "image id" date 

To start interractive terminal session with container
Run 
docker exec --interactive --tty "container id" bash 

