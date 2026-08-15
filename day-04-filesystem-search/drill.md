#  Day 4

## Task
Find every .conf file under /etc, find every file larger than 1MB in /var, then
report total disk usage of /home and remaining free space on the root filesystem.

## Commands run, in order

find /etc -name "*.conf"
find /var -type f -size +1M
du -sh /home
df -h /
