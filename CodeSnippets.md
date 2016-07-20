## Code





| Command  | When to use it |
| -------- | -------------- |
| create   | Create a new container |
| attach   | Attach to a running container |
| kill     | Kill a running container |
| ps       | List containers |
| rename   | Rename a container |
| restart  | Restart a container |
| rm       | Remove one or more containers |
| run      | Run a command in a new container |
| logs     | Fetch the logs of a container |
| start    | Start one or more stopped containers |
| stats    | Display a live stream of container(s) resource usage statistics |
| stop     | Stop a running container |
| cp       | Copy files/folders between a container and the local filesystem |
| diff     | Inspect changes on a container's filesystem |
| exec     | Run a command in a running container |
| pause    | Pause all processes within a container |
| top      | Display the running processes of a container |
| unpause  | Unpause all processes within a container |
| update   | Update resources of one or more containers |


| Command  | When to use it |
| -------- | -------------- |
| commit   | Create a new image from a container's changes | 
| build    | Build an image from a Dockerfile |
| history  | Show the history of an image |
| images   | List images |
| rmi      | Remove one or more images |
| port     | List port mappings or a specific mapping for the CONTAINER |
| pull     | Pull an image or a repository from a registry |
| push     | Push an image or a repository to a registry |
| save     | Save an image(s) to a tar archive |
| load     | Load an image from a tar archive or STDIN |
| search   | Search the Docker Hub for images |
| tag      | Tag an image into a repository |

| Command  | When to use it |
| -------- | -------------- |
| events   | Get real time events from the server |
| export   | Export a container's filesystem as a tar archive |
| import   | Import the contents from a tarball to create a filesystem image |
| info     | Display system-wide information |
| inspect  | Return low-level information on a container or image |
| login    | Register or log in to a Docker registry |
| logout   | Log out from a Docker registry |
| network  | Manage Docker networks |
| version  | Show the Docker version information |
| volume   | Manage Docker volumes |
| wait     | Block until a container stops, then print its exit code |


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
$ docker images			//Listing the most recently created images
$ docker images java	//Listing images by name 
$ docker images java:8	//Listing images by name and tag
$ docker images --digests	//Listing the full length image ID
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
