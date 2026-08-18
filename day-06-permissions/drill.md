# drill.md — Day 6

## Task
Create a script file and set it to rwxr-xr-x using all three chmod methods
(relative, assignment, octal) in turn, confirming the result with ls -l after
each change.

## Commands run, in order

touch myscript.sh
chmod +x myscript.sh
ls -l myscript.sh
chmod u=rwx,g=rx,o=rx myscript.sh
ls -l myscript.sh
chmod 755 myscript.sh
ls -l myscript.sh
