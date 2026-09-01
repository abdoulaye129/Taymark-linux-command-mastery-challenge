#  Day 21 drill

## Task
Find the PID of a running process by name, view it in top, show it as part of
the process tree, and identify which process is using port 80.

## Commands run, in order

pgrep nginx
top
pstree -p
sudo lsof -i :80
