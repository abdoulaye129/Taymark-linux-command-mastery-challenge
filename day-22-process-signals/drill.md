#  Day 22 drill

## Task
Start a long-running command in the background, suspend it, resume it in the
background, then start a second one that survives you logging out, using
nohup.

## Commands run, in order

sleep 300 &
Ctrl+Z
bg
jobs
nohup sleep 300 &
disown
