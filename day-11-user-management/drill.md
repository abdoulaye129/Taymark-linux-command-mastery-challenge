#  Day 11 drill

## Task
Create a new user with a home directory and Bash shell, set their password,
add them to a secondary group, rename the account, then remove it along with
its home directory.

## Commands run, in order

sudo useradd -m -s /bin/bash testuser
sudo passwd testuser
sudo usermod -aG developers testuser
sudo usermod -l testuser2 testuser
sudo userdel -r testuser2
