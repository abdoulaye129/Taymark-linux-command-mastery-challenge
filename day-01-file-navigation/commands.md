# Commands Covered

1. `pwd` shows you exactly which folder you are in right now. I always run this first when I open a terminal and forget where I am.

2. `ls` lists the names of files and folders inside your current directory. It just gives you the names, nothing more.

3. `ls -l` gives you the full details. It shows who owns each file, who can read or write it, how big it is, and when it was last changed.

4. `ls -a` shows everything, including hidden files that start with a dot. The basic `ls` command hides those by default.

5. `ls -la` does both at once. It shows all files with all the full details. This is the one I use when I need the whole picture.

6. `ls -lh` works like `ls -l`, but it changes file sizes into something easy to read, like "2.1M" instead of a long number of bytes.

7. `cd` with a full path (starting from `/`, like `/var/log`) takes you straight to that folder, no matter where you are right now.

8. `cd ..` moves you up one level, back to the parent directory.
9. `cd ~` takes you directly to your home directory (like `/home/yourname`). It is a quick way to reset and start over.

10. `cd -` swaps you back to the last folder you were in. I use this to flip between two folders without typing the long path again.
