### Copy and paste the full code of your backup.sh script. 
```
#!/bin/bash 
# Automated Backup Script for CloudNova Technologies 
SOURCE_DIR="app-data" 
BACKUP_DIR="backups" 
TIMESTAMP=$(date +"%Y%m%d_%H%M%S") 
echo "Initiating automated backup..." 
# Create the backup directory if it does not exist 
mkdir -p $BACKUP_DIR 
# Compress the source directory into a tarball (.tar.gz) 
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR 
echo "Backup completed successfully at $TIMESTAMP!"
```

### Explain what the chmod +x command did to the file.
The chmod +x command is used give a file permission to be executed without this command the file we want to execute can't be executed so we need to give permission first so chmod +x is the one responsible for this. 

### Copy the cron expression you used (0 2 * * * /root/backup.sh) and break down what each of the five time-fields means (Minute, Hour, Day of Month, Month, Day of Week).

| Field | Value | Simple Meaning |
|---|---|---|
| Minute (0-59) | `0` | On the hour exactly (no extra minutes) |
| Hour (0-23) | `2` | At 2 AM |
| Day of month (1-31) | `*` | Every day |
| Month (1-12) | `*` | Every month |
| Day of week (0-7) | `*` | Every day of the week |
| Command | `/root/backup.sh` | Run this backup script |
