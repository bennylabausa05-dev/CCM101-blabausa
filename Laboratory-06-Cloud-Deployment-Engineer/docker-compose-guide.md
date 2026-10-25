## What does the services: block do?
Think of services: as the guest list for your application. Each name under it is one container that Docker must create, and the settings below each name describe how to run it.

## How did the Nextcloud app container know how to find the database container?
It works like a phone book: Docker Compose gives every service a name on a shared private network, and MYSQL_HOST=database tells Nextcloud which name to call. The name matches the database service in the YAML, so Nextcloud reaches MariaDB without needing an IP address.

## What is the difference between docker run and docker-compose up -d?
docker run is like cooking one dish at a time by hand, while docker-compose up -d is like following a full recipe that prepares everything together. Compose reads the YAML file, builds the network, volumes and both containers, and -d keeps it all running in the background.
