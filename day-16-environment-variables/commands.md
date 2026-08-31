#  Day 16: Environment Variables

1. **printenv** — prints every environment variable currently set in your session, one per line.

2. **printenv HOME** — same command, but pointed at a single named variable, so you only get that one value back instead of the full list.

3. **echo $VAR** — a shell-level way to print a single variable's value, using the `$` to tell the shell you want its contents rather than the literal text "VAR".

4. **export** — takes a shell variable and marks it as an environment variable, meaning it gets passed down to any child processes or programs launched from that shell.

5. **unset** — removes a variable entirely from the current session, whether it was exported or not.

6. **env** — similar to `printenv` with no arguments, listing all environment variables. It can also run a command with a modified environment, which `printenv` can't do.

7. **source** — executes a script in the current shell rather than a new subshell, which matters because any variables it sets actually stick around in your session afterward.

8. **echo $PATH** — prints the current value of `PATH`, the list of directories the shell searches through when you type a command name without giving its full path.

9. **export PATH=$PATH:** — appends a new directory to the existing `PATH` rather than replacing it outright. The trailing colon-and-path is what adds to the list instead of wiping it.

10. **cat /etc/environment** — reads the system-wide environment variable file directly, which is where variables get set for every user's session, not just the current one.
