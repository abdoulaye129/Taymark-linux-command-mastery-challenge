# Day 7

## Task
Create a shared project folder, apply the SGID bit so new files inherit its
group, then audit the whole system for unexpected SUID binaries.

## Commands run, in order

mkdir /shared/project
chgrp devteam /shared/project
chmod g+s /shared/project
ls -ld /shared/project
find / -perm /4000 -type f 2>/dev/null
