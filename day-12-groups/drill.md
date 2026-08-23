# drill.md — Day 12

## Task
Create a group named devs, add two users to it, confirm membership with
getent, remove one member, then delete the group entirely.

## Commands run, in order

sudo groupadd devs
sudo gpasswd -a alice devs
sudo gpasswd -a bob devs
getent group devs
sudo gpasswd -d bob devs
getent group devs
sudo groupdel devs
