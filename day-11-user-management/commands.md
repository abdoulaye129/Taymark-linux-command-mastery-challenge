#  Day 11: Creating & Managing Users

1. **useradd** — creates a new user account at a low level. On its own it's fairly bare-bones — no home directory or shell is guaranteed unless you specify them.

2. **useradd -m** — same as `useradd`, but also creates a home directory for the new user, which is usually what you actually want.

3. **useradd -m -s** — creates the user, their home directory, and sets their login shell in one go (e.g. `useradd -m -s /bin/bash newuser`), so the account is actually usable right away.

4. **adduser** — a more user-friendly, interactive wrapper around `useradd` on Debian-based systems. It walks you through setting a password and other details instead of requiring every flag up front.

5. **passwd** — sets or changes a user's password. Run without a username it changes your own; run with one (as root or via `sudo`) it changes someone else's.

6. **usermod -aG** — adds a user to an additional group without removing them from any group they're already in. The `-a` (append) matters here — leaving it off can wipe their existing group memberships.

7. **usermod -s** — changes a user's login shell after the account already exists, without needing to recreate it.

8. **usermod -l** — renames an existing user's login name, which is useful when an account was set up wrong or someone's name changes, without deleting and recreating the whole account.

9. **userdel** — deletes a user account. On its own, this leaves their home directory and files behind.

10. **userdel -r** — deletes a user account and removes their home directory and mail spool along with it, for a clean, complete removal.
