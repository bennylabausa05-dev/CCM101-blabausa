Automation is important when you manage hundreds of cloud servers because doing the work by hand takes too long. 
Logging into every server to run backups, install updates, or clean files could take days, and people often make mistakes when they repeat the same task. 
A script does the same steps on every server, saves time, and keeps all servers the same, even at night when nobody is working.
But automation can also be dangerous. If a script has a bad typo, it repeats that mistake everywhere. 
For example, if a variable is empty, a delete command like rm -rf "$BACKUP_DIR"/* could end up deleting far more than intended. On one server that is bad, but scheduled on 1,000 servers, it could erase all of them at once, even the backups. 
To stay safe, teams test on one server first, roll out changes slowly, use safety options like set -e, and keep backups on a different server.
The tool you choose also matters. A Bash script is a list of steps: you tell the computer what to do, one step after another, and you must check for errors yourself. 
That is why our backup script said “success” even though tar failed. A Docker Compose file is different. It describes the result you want, such as which containers, ports, and storage should exist, and Docker figures out how to build it. This makes Compose more predictable and easy to repeat, while Bash works well for jobs like backups. 
Used together, cron can run the Bash scripts and Compose can keep the services running, which gives teams reliable automation with fewer costly mistakes.

My Understanding About Cloud computing from lab 1-9 is fun and difficult because at first i don't actually understand what im doing but throughout the activity i've done I learned Slowly although not all at least I learn something new.
Throughout the this semester i enjoy more about Deployment because it is easy to deploy and fast in just a few commands your docker container is already made.
