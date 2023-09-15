

*checking version*
``` bash
docker -v
docker --version
```

*running a container*
``` bash
docker run --name mydocker busybox:latest
```
- name : refers to name of the container
- busybox:latest : image we are intrested in . the tag latest signifies that it will pull from registry the latest image of Busybox ,  is a tiny little Linux binary that is meant for embedded systems

*pausing a container*
``` bash
docker container pause mydocker
docker ps -a
docker ps --all
```
*unpausing*
```bash
docker container unpause mydocker
```
*stoping*
```bash
docker container stop mydocker
```
*running a container with -dit*
``` bash
docker run -dit --name my_container busybox:latest
```
- d: also --detach , means the container runs in detached mode i.e the background
- i: also --interacive , means that the container will accept input and provide output
- -t: also --tty , means our container is in interactive mode , we will usually need to provide a terminal for getting the output

*getting inside a container*
``` bash
docker exec -i -t my_container sh
```
-sh : sh can take input from either a keyboard or a file 
