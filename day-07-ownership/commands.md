# Day 7: Ownership & Special Bits

1. **chown** — changes which user owns a file. On its own it only touches the owner, not the group.

2. **chown user:group** — changes owner and group in a single command, which is faster than running `chown` and `chgrp` separately.

3. **chown -R** — applies an ownership change recursively through every file and subdirectory, not just the top-level target.

4. **chgrp** — changes only the group associated with a file, leaving the owner untouched.

5. **chmod u+s (SUID)** — sets the SUID bit on an executable, which makes it run with the permissions of the file's owner rather than whoever launched it. This is what lets tools like `passwd` write to files a normal user otherwise couldn't touch.

6. **chmod g+s (SGID)** — on a directory, this makes new files created inside automatically inherit that directory's group instead of the creating user's default group. Useful for shared team folders.

7. **chmod +t (sticky bit)** — on a shared directory, restricts deletion so users can only remove or rename their own files, even if they have write access to the folder. `/tmp` is the classic example.

8. **find -perm /4000** — searches the filesystem for anything with the SUID bit set, which is a standard first step in auditing a system for unexpected privilege escalation risks.

9. **getfacl** — displays a file's full Access Control List, which can grant permissions to specific users or groups beyond the standard owner/group/other model.

10. **setfacl -m** — modifies a file's ACL to add or change a permission entry for a specific user or group, without disturbing the regular owner/group/other permissions.
