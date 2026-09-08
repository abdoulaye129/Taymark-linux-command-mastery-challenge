# Day 30 · Capstone

## Task
CAPSTONE PROJECT. Ship one Bash script that connects to a remote server over
SSH, deploys a file with the correct ownership and permissions, restarts the
relevant service, verifies it is healthy using systemctl and journalctl, and
logs the entire run. Then walk a peer through it end to end, using only
commands from this challenge.

## Commands run, in order

ssh-copy-id user@remotehost
nano deploy-and-check.sh
chmod +x deploy-and-check.sh
./deploy-and-check.sh
crontab -e
crontab -l
