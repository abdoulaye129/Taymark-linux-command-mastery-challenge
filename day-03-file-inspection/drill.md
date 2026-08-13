# drill.md — Day 3

## Task
Pick a log file on the system. View it fully with `cat`, page through it with `less`,
show the first and last 15 lines, count its lines, identify its file type, and inspect
its full metadata with `stat`.

## Commands run (in order)

cat /var/log/syslog
less /var/log/syslog
head -n 15 /var/log/syslog
tail -n 15 /var/log/syslog
wc -l /var/log/syslog
file /var/log/syslog
stat /var/log/syslog
