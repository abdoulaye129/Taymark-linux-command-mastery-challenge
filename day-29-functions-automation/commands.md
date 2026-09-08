#  Day 29: Functions, Arguments & Automation

1. **function_name() { }** — defines a reusable block of code you can call by name, instead of retyping the same commands over and over across a script.

2. **$1 / $2 positional args** — refers to the arguments passed into a script or function, in order. `$1` is the first one, `$2` the second, and so on.

3. **$# / $* / $@** — `$#` counts how many arguments were passed, `$*` and `$@` both expand to all of them, with a subtle quoting difference between the two.

4. **$0** — refers to the name of the script itself, as it was called. Useful for logging or error messages that need to reference the script by name.

5. **exit codes ($?)** — every command leaves behind an exit code when it finishes, and `$?` captures the most recent one. Zero means success, anything else means something went wrong.

6. **crontab syntax** — the five-field time format cron uses to decide when a job runs — minute, hour, day, month, weekday. Cryptic-looking until you've written a few.

7. **cron scheduling (0 * * * *)** — a specific example: this pattern runs a job at the top of every hour, on the hour, every day.

8. **nohup script.sh &** — runs a script in the background and makes sure it survives even after you log out, combining two ideas from Day 22 into one line.

9. **trap** — catches a signal sent to a script (like Ctrl+C) and runs custom cleanup code instead of letting the script just die abruptly.

10. **logger** — writes a message straight into the system log, which is genuinely useful for scripts that need to leave a trail for later auditing.
