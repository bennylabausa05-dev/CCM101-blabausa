### Mission Overview
Congratulations! After successfully guiding our clients through multi-cloud evaluations, you have been 
promoted to the Cloud-Native Engineering Team at CloudNova Technologies. 
Modern cloud computing is no longer just about renting Virtual Machines (VMs) from AWS or Azure. Today's 
enterprise applications are built using lightweight, portable, and lightning-fast technologies called Containers. 
Your new mission is to understand the shift from traditional virtualization to containerization. 
Using the KillerCoda Playground, you will step into the shoes of a Cloud-Native Engineer. You will research the 
differences between VMs and containers, execute your very first Docker commands, and deploy a live, 
containerized web server in seconds.

### Objectives
* Differentiate between traditional Virtual Machines (VMs) and Containers. 
* Access a Docker-enabled cloud environment using KillerCoda. 
* Execute fundamental Docker CLI (Command Line Interface) commands. 
* Pull, run, manage, and terminate a containerized application (Nginx). 
* Create professional technical documentation of container operations using Markdown. 
* Continue developing a well-organized GitHub Cloud Computing Portfolio.

### Docker Commands Executed

- Check Versions and other Info: `docker --version && sudo systemctl is-active docker && docker ps -a`
- to download the latest official Nginx image from Docker Hub: `docker pull nginx`
- Run the container in detached mode and map port 8080 on your host 80 inside container: `docker run -d --name my-nginx -p 8080:80 nginx`
- Confirm the container is running, list running containers: `docker ps`
- Verify that the web server is actually running by sending an HTTP request locally: `curl http://localhost:8080`
- this permanently deletes the stopped container and its writable layer: `docker rm my-nginx`
- this sends a SIGTERM (then SIGKILL if needed) to gracefully shut down the container's main process without deleting the container itself: `docker stop my-nginx`
- Confirm the container is stopped: `docker ps -a`

### Skills Learned
Installing, running, and managing Docker containers (pull, run, stop, remove); using port mapping to connect a container to the outside network; testing a running service with curl; understanding the difference between images and containers; comparing VMs vs. containers on speed, resource use, and isolation; writing clear technical documentation; and understanding how containers help Dev and Ops teams work together more smoothly.

### Challenges Encountered 
There is so many challenges that i encountered but some of the major problem is that the appropriate approach how to do this especially that I have no knowledge about docker and i am only basing on the modules that discussed but I research About it and found some Answers to it so it helps me a lot.
