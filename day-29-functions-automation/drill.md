# Day 29 drill

## Task
Turn yesterday's script into a reusable function that accepts a service name
as an argument, checks its status, restarts it if stopped, and schedule it to
run hourly with cron.

## Commands run, in order

nano service-checker.sh
chmod +x service-checker.sh
./service-checker.sh nginx
crontab -e
crontab -l
