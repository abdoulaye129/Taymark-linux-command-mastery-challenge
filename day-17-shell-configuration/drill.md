# Day 17 drill

## Task
Add a permanent environment variable and a custom alias to your .bashrc,
reload it without opening a new terminal, and confirm both persist in a
fresh session.

## Commands run, in order

echo 'export MYVAR="persisted"' >> ~/.bashrc
echo "alias ll='ls -la'" >> ~/.bashrc
source ~/.bashrc
echo $MYVAR
ll
bash
echo $MYVAR
ll
