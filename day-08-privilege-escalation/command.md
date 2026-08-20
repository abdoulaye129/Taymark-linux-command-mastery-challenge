# commands.md — Day 8: Privilege Escalation & Identity

1. **sudo** — runs a single command with elevated (usually root) privileges, without having to log in as another user. This is the standard, auditable way to do admin work rather than staying logged in as root the whole time.

2. **sudo -i** — opens a full root login shell, as if you'd logged in as root directly. More persistent than a one-off `sudo` command, so it's worth using sparingly.

3. **sudo -u** — runs a command as a specific user rather than root (e.g. `sudo -u deploy whoami`), which is useful when you need another account's permissions, not necessarily root's.

4. **sudo !!** — re-runs the previous command, prefixed with `sudo`. The one I'd reach for the second a command fails with a permission error, instead of retyping the whole thing.

5. **sudo -l** — lists exactly which commands your account is permitted to run with `sudo`, and under what conditions. Good for checking your own access, or auditing someone else's.

6. **visudo** — the safe way to edit the sudoers file. It locks the file while you work and checks the syntax before saving, so a typo can't lock everyone out of `sudo`.

7. **su** — switches to another user account, prompting for that user's password. Without a username it defaults to root.

8. **su -** — same as `su`, but also loads that user's full environment (shell, home directory, path), so it behaves like an actual fresh login rather than just borrowing their permissions.

9. **whoami** — prints the username of whoever is currently running the shell. A quick sanity check after switching users or using `sudo`.

10. **id** — prints your full identity: user ID, group ID, and every group you belong to. More detail than `whoami`, and useful for confirming group membership actually took effect.
