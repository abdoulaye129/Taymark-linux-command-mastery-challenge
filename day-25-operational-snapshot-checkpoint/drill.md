# Day 25 · Checkpoint

## Task
CHECKPOINT. Build a one-screen operational snapshot of a server covering
uptime, memory, the status of three key services, and any scheduled cron
jobs.

## Commands run, in order

uptime
free -h
systemctl status nginx
systemctl status ssh
systemctl status cron
crontab -l
