# NGINX_Docker
NGINX Load Balancer Configuration for Docker



## *Part 2* | NGINX Config and DockerFile

###  Here in this project i'll be dockerizing a Node.js application and then deploy 10 containers in a swarm cluster, load balance them behind a single IP with Nginx and then finally conclude with scaling them up and down also visualize the containers in a better way.  

### So the main purpose of this project is not the NodeJs app itself, but rather to  deployi an Node.js app to 10 containers in a swarm then load balance them.

## Content

### - <a title="Part 1" href="https://github.com/cstoicescu/WhoAmI_NodeJs_Docker" target="_blank">Part 1</a> 
### - <a title="Part 2" href="https://github.com/cstoicescu/NGINX_Docker" target="_blank">Part 2</a> 
### - <a title="Part 3" href="https://github.com/cstoicescu/Vagrant_DockerSwarm" target="_blank">Part 3</a> 
 
 ## Final Result after Deploy:  
 https://user-images.githubusercontent.com/53979557/120241164-d6bd8a80-c26a-11eb-81dd-e749cd34b591.gif


 ### Second Step:  Building the NGINX image from github repo and pushing it to Docker Hub

$docker build -t catalin-nginx-balancer-conf:1.0 https://github.com/cstoicescu/NGINX_Docker.git 

$docker run catalin-nginx-balancer-conf:1.0

$docker container ls

$docker login

$docker push cstoicescu/catalin-nginx-balancer-conf:tagname   

### At this point, your DockerHub should have the 2 repos ( Nodejs and Nginx )  

<img src="https://i.imgur.com/wWhLb3z.jpg" />  
