#  Day 12: Groups & Access Circles

1. **groupadd** — creates a new group on the system, which you can then add users to for shared access control.

2. **groupdel** — deletes a group entirely. This only removes the group itself, not any users who were members of it.

3. **gpasswd -a** — adds a user to a group. Functionally similar to `usermod -aG`, but it's the dedicated group-management tool rather than a user-management one repurposed for the job.

4. **gpasswd -d** — removes a user from a group, without touching their other group memberships or the account itself.

5. **getent group** — queries the system's group database and prints an entry for a specific group, showing its name, GID, and member list.

6. **getent passwd** — same idea as `getent group`, but for user accounts — pulls a specific user's entry from the system's password database.

7. **groups** — lists every group a given user belongs to, which is the quickest sanity check after adding or removing someone from a group.

8. **id -Gn** — prints just the group names a user belongs to, in plain text form, which is a cleaner alternative to parsing the full output of `id`.

9. **newgrp** — temporarily switches your active primary group for the current session, without permanently changing your account's group settings.

10. **cat /etc/group** — reads the raw group database file directly, showing every group on the system and its members. Useful when you want the full picture rather than querying one group at a time.
