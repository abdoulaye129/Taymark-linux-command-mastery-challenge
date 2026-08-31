#  Day 17: Persisting Configuration

1. **nano ~/.bashrc** — opens your personal shell startup file in the nano editor, where you'd add anything you want set up automatically every time you open a new terminal.

2. **source ~/.bashrc** — re-runs `.bashrc` in your current shell without needing to close and reopen the terminal, so changes take effect immediately.

3. **cat ~/.bash_profile** — reads a different startup file that runs specifically for login shells, as opposed to `.bashrc` which runs for interactive non-login shells.

4. **sudo nano /etc/environment** — edits the system-wide environment file, which sets variables for every user on the machine rather than just one account.

5. **sudo nano /etc/bash.bashrc** — edits the system-wide Bash configuration that applies to every user's shell, similar in spirit to a personal `.bashrc` but scoped to the whole system.

6. **alias** — creates a shortcut name for a longer command (e.g. `alias ll='ls -la'`), which is one of the simplest ways to save yourself repetitive typing.

7. **unalias** — removes a previously defined alias from the current session.

8. **type** — tells you what a given command name actually resolves to — whether it's a built-in, an alias, a function, or a file on disk — which is useful when a command isn't behaving the way you expect.

9. **which** — shows the full path to the executable that would run if you typed a given command name, based on your current `PATH`.

10. **whereis** — similar to `which`, but broader — it can also show a command's manual page and source files, not just its binary location.
