# Day 16

## Task
Set a temporary environment variable, confirm it exists, unset it, then add a
directory to your PATH for the current session only and prove the shell can
now find a script inside it.

## Commands run, in order

export TESTVAR="hello"
echo $TESTVAR
unset TESTVAR
echo $TESTVAR
mkdir -p ~/myscripts
echo 'echo "script ran"' > ~/myscripts/hello.sh
chmod +x ~/myscripts/hello.sh
export PATH=$PATH:~/myscripts
hello.sh
