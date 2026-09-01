# Day 20 · Checkpoint: Text Processing & Pipes
## commands covered
1. **grep** — searches text for lines matching a pattern and prints just those lines. The workhorse of log-hunting.

2. **grep -r** — runs that same search recursively through every file in a directory tree, not just one file at a time.

3. **grep -i** — makes the search case-insensitive, so "Error" and "error" both count as a match.

4. **sort** — arranges lines alphabetically by default. Simple, but it's the building block for a lot of pipeline work.

5. **sort -n** — sorts numerically instead of alphabetically. Without this flag, "10" sorts before "2," which trips people up constantly.

6. **uniq** — removes duplicate lines, but only if they're sitting next to each other. That's why it almost always follows a `sort` first.

7. **cut -d',' -f** — pulls out a specific column from delimited text (like a CSV), using `-d` to set the delimiter and `-f` to pick the field number.

8. **awk '{print $1}'** — prints the first column of each line, whitespace-delimited by default. Awk can do far more, but this is the entry point.

9. **sed 's/old/new/g'** — a command-line find-and-replace, the same logic as Vim's `:%s`, just usable directly in the terminal or inside a script.

10. **pipe chains (|)** — connects one command's output straight into the next command's input, which is how a handful of simple tools combine into a real pipeline.
