1. ### **List Running Containers**
root@ubuntu:~$ docker ps
CONTAINER ID   IMAGE     COMMAND                  CREATED         STATUS         PORTS                                     NAMES
931b3995df9f   nginx     "/docker-entrypoint.…"   5 minutes ago   Up 5 minutes   0.0.0.0:8080->80/tcp, [::]:8080->80/tcp   my-nginx

2. ### **Stop running container**
root@ubuntu:~$ docker stop my-nginx
my-nginx

3. ### **Verify It is Stopped**
root@ubuntu:~$ docker ps -a
CONTAINER ID   IMAGE     COMMAND                  CREATED         STATUS                      PORTS     NAMES
931b3995df9f   nginx     "/docker-entrypoint.…"   6 minutes ago   Exited (0) 12 seconds ago             my-nginx

4. ### **Remove The Container completely**
root@ubuntu:~$ docker rm my-nginx
my-nginx

5. ### **Verify again If Container is Deleted**
root@ubuntu:~$ docker ps -a
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES



## Commands Used 

1.**List running containers**
   Run `docker ps` — this shows all currently running containers, including their container ID, image, status, and port mappings. Confirm `my-nginx` appears with status "Up".
2. **Stop the running container** 
   Run `docker stop my-nginx` — this sends a SIGTERM (then SIGKILL if needed) to gracefully shut down the container's main process without deleting the container itself.
3. **Verify it is stopped**
   Run `docker ps -a` — the `-a` flag shows all containers regardless of state. You should see `my-nginx` listed with status "Exited" instead of "Up".
4. **Remove the container completely**
   Run `docker rm my-nginx` — this permanently deletes the stopped container and its writable layer. Run `docker ps -a` again afterward to confirm it's gone from the list.






   
