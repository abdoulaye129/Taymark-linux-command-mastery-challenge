# Day 5 · Checkpoint

## Task
CHECKPOINT. Create a symbolic link to a config file, resolve its real path, print a
two-level tree of /etc, and explain to a peer, in your own words, the difference
between a hard link and a symbolic link.

## Commands run, in order

ln -s /etc/hosts ~/hosts-link
readlink ~/hosts-link
realpath ~/hosts-link
tree -L 2 /etc
