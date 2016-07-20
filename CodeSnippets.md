## Code

Docker management commands
* Container commands
* Image commands
* Hub and registry commands
* Network and connectivity commands
* Shared data volume commands
* Swarm node commands
* Swarm swarm commands
* Swarm service commands

[Detailed commands](http://docs.master.dockerproject.org/engine/reference/commandline/)


[Dockerfile reference](http://docs.master.dockerproject.org/engine/reference/builder/)


### Sample Docker commands 
```
// we pull a base Docker image called busybox
// just like in the official Hello-World-example
sudo docker pull busybox
 
// let's check which images we have 
// we should see the image busybox
sudo docker images
 
//now we make changes to a container of this image
// in this case we make a new folder
//sudo docker run busybox mkdir /home/test
 
//let's check which containers we now have
//note that the container stops after each command
//we should see a busybox container with our command
sudo docker ps -a
 
//now we can commit this changed container
// this will create a new image called busybox-1
//you see the <CONTAINER ID> with the command above
sudo docker commit <CONTAINER ID> busybox-1
 
// let's check which images we have now
// we should see the image busybox and busybox-1
sudo docker images
 
// to see the difference between both images we
// can use the following check for folders:
sudo docker run busybox [ -d /home/test ] && echo 'Directory found' || echo 'Directory not found'
sudo docker run busybox-1 [ -d /home/test ] && echo 'Directory found' || echo 'Directory not found'


## Export
// <CONTAINER ID>
docker ps -a

//export a container 
docker export <CONTAINER ID> /home/export.tar

## Save
//docker images
docker images


//To save an image
docker save busybox-1 > /home/save.tar


## difference
// first we see which containers we have
sudo docker ps -a
 
// now we remove all of them
sudo docker rm <CONTAINER ID>
 
// now we see which images we have
sudo docker images
 
// and we remove them too
sudo docker rmi busybox-1
sudo docker rmi busybox

// import the exported tar ball:
docker load < /home/save.tar

// check the available images
sudo docker images

// and check if a new container made from this image contains our folder (it does!)
sudo docker run busybox-1 [ -d /home/test ] && echo 'Directory found' || echo 'Directory not found'
```

##create   
##attach   
##kill     	
##ps       	
##rename   	
##restart  	
##rm       	
##run      	
##logs     	
##start    
##stats    
##stop     
##cp       
##diff     
##exec     
##pause    
##top      
##unpause  
##update   

##commit   
##build    
##history  
##images   
```docker
$ docker images											//Listing the most recently created images
$ docker images java									//Listing images by name 
$ docker images java:8									//Listing images by name and tag
$ docker images --digests								//Listing the full length image ID
$ docker images --filter "dangling=true"				#Filtering
$ docker images --format "{{.ID}}: {{.Repository}}"		#Formatting
```
##rmi      
##port     
##pull     
##push     
##save     
##load     
##search   
##tag      

##events   
##export   
##import   
##info     
##inspect  
##login    
##logout   
##network  
##version  
##volume   	
##wait     	




### Sample Docker files
```

# Comment
# INSTRUCTION arguments

RUN echo 'we are running some # of cool things'


# directives
tive=value

FROM ImageName

FROM windowsservercore
COPY testfile.txt c:\\
RUN dir c:\

FROM <image>
FROM <image>:<tag>
FROM <image>@<digest>

MAINTAINER <name>


RUN /bin/bash -c 'source $HOME/.bashrc ; echo $HOME'


FROM ubuntu
CMD echo "This is a test." | wc -

LABEL "com.example.vendor"="ACME Incorporated"
LABEL com.example.label-with-value="foo"
LABEL version="1.0"
LABEL description="This text illustrates \
that label-values can span multiple lines."


ENV myName="John Doe" myDog=Rex\ The\ Dog \     myCat=fluffy

ENV myName John Doe
ENV myDog Rex The Dog
ENV myCat fluffy


ADD hom* /mydir/        # adds all files starting with "hom"
ADD hom?.txt /mydir/    # ? is replaced with any single character, e.g., "home.txt
ADD test relativeDir/          # adds "test" to `WORKDIR`/relativeDir/
ADD test /absoluteDir/         # adds "test" to /absoluteDir/


COPY hom* /mydir/        # adds all files starting with "hom"
COPY hom?.txt /mydir/    # ? is replaced with any single character, e.g., "home.txt"
COPY test relativeDir/   # adds "test" to `WORKDIR`/relativeDir/
COPY test /absoluteDir/  # adds "test" to /absoluteDir/


docker run -i -t --rm -p 80:80 nginx


FROM ubuntu
ENTRYPOINT ["top", "-b"]
CMD ["-c"]


FROM debian:stable
RUN apt-get update && apt-get install -y --force-yes apache2
EXPOSE 80 443
VOLUME ["/var/www", "/var/log/apache2", "/etc/apache2"]
ENTRYPOINT ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]


FROM ubuntu
RUN mkdir /myvol
RUN echo "hello world" > /myvol/greeting
VOLUME /myvol

USER daemon

WORKDIR /path/to/workdir
WORKDIR /a
WORKDIR b
RUN pwd

FROM busybox
ARG user1=someuser
ARG buildno=1

FROM busybox
USER ${user:-some_user}
ARG user
USER $user


ONBUILD ADD . /app/src
ONBUILD RUN /usr/local/bin/python-build --dir /app/src


STOPSIGNAL signal


HEALTHCHECK --interval=5m --timeout=3s  CMD curl -f http://localhost/ || exit 1


FROM windowsservercore
SHELL ["powershell","-command"]
RUN New-Item -ItemType Directory C:\Example
ADD Execute-MyCmdlet.ps1 c:\example\
RUN c:\example\Execute-MyCmdlet -sample 'hello world'

```
