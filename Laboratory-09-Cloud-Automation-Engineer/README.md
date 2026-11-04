# Laboratory 09 - Cloud Automation Engineer

## Mission Overview

This laboratory demonstrates how Bash scripts and Linux cron jobs can automate routine cloud operations tasks. A script is created to compress a sample data directory into a timestamped backup archive and is scheduled to run daily.

## Objectives

- Understand Bash scripts, variables, and cron jobs.
- Create sample data for a backup exercise.
- Write and execute a Bash backup script.
- Change file permissions using `chmod`.
- Schedule automated backups using `crontab`.
- Document the script and cron schedule.

## Commands Executed

- `mkdir` - Create directories.
- `echo` - Create a sample data file.
- `nano` - Edit scripts and documentation.
- `chmod +x backup.sh` - Make the script executable.
- `./backup.sh` - Run the backup script.
- `ls -lh backups/` - Inspect generated backup files.
- `tar -tzf` - List the contents of a compressed archive.
- `crontab -l` - Display scheduled cron jobs.
- `env EDITOR=nano crontab -e` - Edit the cron schedule.

## Skills Learned

- Bash scripting and variable usage.
- Linux file permissions.
- File compression and backup verification.
- Cron scheduling.
- Automation documentation and version control.

## Screenshots

- `screenshots/script-execution.png`
- `screenshots/cron-schedule.png`
