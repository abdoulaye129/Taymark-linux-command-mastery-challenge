#  Day 19 drill

## Task
In a 50-line config file, jump straight to line 10, search for a keyword,
jump between all matches, then replace every occurrence of one word with
another across the whole file.

## Commands run, in order

vim config-sample.txt
:10
/timeout
n
n
:%s/timeout/duration/g
ZZ
