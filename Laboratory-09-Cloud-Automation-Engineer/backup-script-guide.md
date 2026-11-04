# Backup Script Guide

## Complete Bash Script

The following script creates a timestamped compressed archive of the `app-data` directory.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies
SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

mkdir -p "$BACKUP_DIR"
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

## File Permissions: `chmod +x`

The command `chmod +x backup.sh` adds execute permission to the script, allowing it to be launched with `./backup.sh`. Without execute permission, the operating system normally refuses to run it directly.

## Cron Schedule

The cron expression used in this mission is:

`0 2 * * * /root/backup.sh`

The five time fields mean:

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

Therefore, the script is scheduled to run every day at 2:00 AM.

## How the Script Works

- `SOURCE_DIR` identifies the folder containing the data.
- `BACKUP_DIR` identifies where the backup files are stored.
- `TIMESTAMP` generates a date and time string to make each backup filename unique.
- `mkdir -p` creates the backup directory if it does not already exist.
- `tar -czf` compresses the source directory into a `.tar.gz` archive.

For important production systems, backups should also be checked for errors, stored securely, and tested through restoration.
