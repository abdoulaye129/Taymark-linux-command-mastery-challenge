# Day 15 · Checkpoint: Users & Packages Checkpoint

1. **id <user>** — prints a specific user's UID, GID, and full group membership in one line, without needing to be logged in as that user.

2. **getent passwd <user>** — pulls a specific user's entry from the system's password database, showing their UID, home directory, and shell.

3. **useradd -m -G** — creates a user with a home directory and adds them to one or more supplementary groups in a single command, rather than doing it as two separate steps.

4. **passwd <user>** — sets or changes the password for a specific named account, run by root or via `sudo`.

5. **apt list --installed** — lists every package currently installed via APT, which is the APT-side equivalent of `dpkg -l`.

6. **apt list --upgradable** — shows only the installed packages that have a newer version available, without actually installing anything.

7. **apt update && apt install -y** — chains two commands together: refresh the package index, then install a package without an interactive confirmation prompt. Useful for scripting installs that shouldn't need a person sitting there.

8. **dpkg -l | grep** — lists all installed packages and filters that list down to ones matching a keyword, handy for quickly checking if something specific is installed.

9. **apt autoremove** — clears out leftover dependency packages that nothing installed currently needs, keeping the system tidy after installs and removals.

10. **history** — shows a list of previously run shell commands, which is useful here for reviewing exactly what was done during a provisioning session.
