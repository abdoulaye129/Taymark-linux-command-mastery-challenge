# Day 18 drill

## Task
Open a new file in vim, type three lines of text, save it, reopen it, delete
the middle line, undo the deletion, then save and quit.

## Commands run, in order

vim practice.txt
i
line one
line two
line three
Esc
:wq
vim practice.txt
2G
dd
u
:wq
