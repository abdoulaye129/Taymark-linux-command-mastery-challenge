#  Day 28: Bash Scripting Foundations

1. **#!/bin/bash (shebang)** — the first line of a script, telling the system exactly which interpreter should run it. Without this, your script's just a random text file with no clear instructions.

2. **chmod +x script.sh** — marks the script as executable. Skip this and the system flat-out refuses to run it, even with the shebang sitting right there.

3. **./script.sh** — actually runs the script. The `./` matters — it tells the shell to look in the current directory instead of searching `PATH` for a command with that name.

4. **VAR=value** — assigns a value to a variable inside a script. No spaces around the `=`, which trips up almost everyone the first time.

5. **$() command substitution** — runs a command and captures its output as a value, so you can store it in a variable or use it inline elsewhere.

6. **read -p** — pauses the script and prompts the user for input, storing whatever they type into a variable.

7. **if / elif / else / fi** — the standard conditional structure. `fi` closes it out — backwards spelling of `if`, and yes, that's genuinely the syntax.

8. **-gt / -lt / -eq** — comparison operators for numbers inside an `if` statement — greater than, less than, equal to. Bash won't let you just use `>` and `<` the way you'd expect.

9. **for loop** — repeats a block of commands once for each item in a list, whether that's a range of numbers, a list of files, or anything else you feed it.

10. **while loop** — repeats a block of commands for as long as a condition stays true. Good for anything that should keep running until some state changes.
