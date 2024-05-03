 ## Docker First Setup
 
 [System Requirment](https://docs.docker.com/get-docker/)

 ## Installation Steps
     - Provision the VM with the required resources (OS Platform)  
     - Install the docker 
               * [Mac](https://docs.docker.com/desktop/install/mac-install/)
               * [Windows](https://docs.docker.com/desktop/install/windows-install/)
               * [Linux](https://docs.docker.com/desktop/install/linux-install/)
 3. start the docker ( systemctl start docker )
 4. now create the one file with the name of daemon.json at /etc/docker/ location with below contet 
 
           {
                "insecure-registries" : ["<My_artifactory_IP:Artifactory_Port"]
           }
 5. Now restart the docker service ( systemctl restart docker )
 6. now pull the image from docker hub ( docker pull httpd )
 7. now change the tag of docker
  
                 docker tag httpd 65.0.178.111:8082/docker_virtual/httpd:latest
 8. Now push the image to the docker current reposiroty
    
	       docker push 65.0.178.111:8082/docker_virtual/httpd:latest
