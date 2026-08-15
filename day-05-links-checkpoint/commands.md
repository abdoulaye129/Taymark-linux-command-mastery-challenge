# Day 5 · Checkpoint: Paths, Links & Tree Structures

1. **tree** — prints a directory's contents as a visual, nested tree instead of a flat list, which makes it much easier to see structure at a glance.

2. **tree -L** — same as `tree`, but capped to a specific depth (e.g. `tree -L 2`), so you don't get buried in output on a deeply nested folder.

3. **ln (hard link)** — creates a second name that points to the exact same data on disk as the original file. Delete the original and the data is still there under the link, because they're really the same file underneath.

4. **ln -s (symbolic link)** — creates a shortcut file that points to another file's path, rather than to its data directly. If the original is deleted or moved, the symlink breaks.

5. **readlink** — shows what a symbolic link is actually pointing to, which is useful when you've got a chain of links and want to know the real target.

6. **realpath** — resolves any path — relative, symlinked, or otherwise — down to its full, absolute form. Good for confirming exactly where something lives.

7. **basename** — strips the directory portion off a path and gives you just the filename at the end.

8. **dirname** — does the opposite of `basename`: strips the filename and gives you just the directory path.

9. **pushd / popd** — a pair for jumping between directories and back again. `pushd` saves your current location onto a stack before moving, and `popd` returns you to it.

10. **ls -lt** — lists files in long format, sorted by modification time with the newest first. Useful for spotting whatever was touched most recently in a busy directory.
