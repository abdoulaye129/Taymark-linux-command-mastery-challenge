# Day 15 · Checkpoint

## Task
CHECKPOINT. Provision a complete new team member account (user, groups,
password) and install the three tools they need for their role, in a single
documented sequence.

## Commands run, in order

sudo useradd -m -G developers,docker -s /bin/bash newhire
sudo passwd newhire
id newhire
sudo apt update && sudo apt install -y git curl vim
dpkg -l | grep -E "git|curl|vim"
history | tail -10
