# Day 4: Searching the Filesystem

1. **find -name** — searches a directory tree for files matching a name pattern. This is the command I'd reach for when I know roughly what a file is called but not where it lives.

2. **find -type** — narrows a `find` search to a specific kind of item — `f` for regular files, `d` for directories. Useful for cutting out noise when you only care about one or the other.

3. **find -size** — filters results by file size (e.g. `+1M` for anything over 1MB). Good for hunting down space hogs without eyeballing every file.

4. **find -mtime** — filters by when a file was last modified, counted in days. I'd use this to find anything touched recently, or conversely, anything that's gone stale.

5. **find -perm** — filters by permission bits, which is how you'd flag files with unusually loose or unusually tight access.

6. **locate** — searches a prebuilt index of filenames instead of walking the filesystem live, so it returns results almost instantly. The tradeoff is that the index can be out of date.

7. **updatedb** — manually rebuilds the index that `locate` reads from. Worth running if you've just created files and `locate` isn't finding them yet.

8. **du** — reports how much disk space a file or directory is actually using, broken down by subfolder if you point it at a directory.

9. **du -sh** — same as `du`, but summarised into a single total and shown in human-readable units (K, M, G) instead of raw byte counts.

10. **df -h** — shows how much space is used and free across your mounted filesystems, also in human-readable units. This is the one I'd check first if a system says it's out of disk space.
