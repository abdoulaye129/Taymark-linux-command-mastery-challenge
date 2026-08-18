# Day 6: Reading & Setting Permissions

1. **ls -l (permission string)** — lists files in long format, and the first column of that output (e.g. `-rwxr-xr-x`) is the permission string: file type, then owner/group/other permissions in three-character blocks.

2. **chmod (relative +/-)** — adjusts permissions relative to what's already there, using `+` to add and `-` to remove (e.g. `chmod +x file` just adds execute without touching anything else).

3. **chmod (assignment =)** — sets permissions to an exact value regardless of what was there before (e.g. `chmod u=rwx file` sets the owner's permissions outright, wiping any prior combination).

4. **chmod 755 (octal)** — sets permissions using a three-digit numeric shorthand. 755 means the owner gets read/write/execute, and group/others get read/execute only.

5. **chmod 644 (octal)** — a common one for regular files: owner gets read/write, group and others get read-only. No execute bit anywhere.

6. **chmod 600 (octal)** — locks a file down so only the owner can read or write it, and nobody else has access at all. This is the one I'd use for anything sensitive, like a private key.

7. **chmod -R** — applies a permission change recursively, walking into every file and subdirectory instead of just the target itself.

8. **umask** — sets the default permissions mask applied to newly created files and directories, so you don't have to `chmod` every new file by hand.

9. **umask -S** — shows the current umask in the same symbolic format `ls -l` uses (rwx), which is a lot easier to read than the raw octal umask value.

10. **stat -c '%A %U %G'** — a custom-formatted `stat` call that prints just the permission string, owner, and group — a quick way to check exactly what you need without the rest of the metadata.
