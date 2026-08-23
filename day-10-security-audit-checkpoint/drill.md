# drill — Day 10 · Checkpoint

## Task
CHECKPOINT. Produce a one-page mini security audit of a server: who has logged
in recently, who is logged in right now, which accounts have never logged in,
and every sudo command run in this session.

## Commands run, in order

last -n 20
w
lastlog
history | grep sudo
