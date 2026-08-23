#  Day 10 · Checkpoint: Security Checkpoint & Audit

1. **find / -perm /4000 (SUID audit)** — sweeps the entire filesystem for binaries with the SUID bit set, which is the standard starting point for checking a system hasn't picked up an unexpected privilege escalation path.

2. **last** — shows a history of user logins, pulled from the system's login records, including who logged in, when, and for how long.

3. **lastlog** — shows the most recent login for every user account on the system, which makes it easy to spot accounts that have never logged in at all.

4. **w** — shows who's currently logged in, what they're doing, and how long their session has been idle, all in one view.

5. **who** — a simpler version of `w`, showing just who's logged in and from where, without the extra activity detail.

6. **groups** — lists every group a given user belongs to, which is a quick way to confirm group membership actually took effect after a change.

7. **passwd** — used on its own (without a username) to change your own password; run against another user's name, it changes theirs — something only root or a permitted `sudo` user can do.

8. **chage -l** — shows a user's password aging details: when it was last changed, and when it's due to expire, if an expiry policy is in place.

9. **lastb** — shows failed login attempts, which is one of the first things worth checking if you suspect someone's been trying to brute-force their way in.

10. **history | grep sudo** — filters your shell history down to just the commands that were run with `sudo`, which makes it easy to review exactly what elevated actions happened in a session.
