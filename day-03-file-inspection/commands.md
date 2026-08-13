#  Day 3: Reading & Inspecting Files

1. **cat** — it dumps a file's entire contents straight to the terminal. Great for small files, useless for anything longer than a screen because it just keeps scrolling.

2. **less** — it opens a file page by page so you can scroll up and down at your own pace. Unlike `cat`, it doesn't load the whole file into memory first, which is why it handles huge files without choking.

3. **head** — it shows the first 10 lines of a file by default. Useful when you just want a quick peek at the top of something without opening the whole thing.

4. **head -n** — same idea as `head`, but you tell it exactly how many lines you want (e.g. `head -n 15`). Handy when the default 10 isn't enough or is too many.

5. **tail** — the mirror image of `head`: shows the last 10 lines. This is usually what I reach for when I want to see the most recent entries in a log.

6. **tail -f** — it follows a file live, printing new lines as they're written. This is the one I'd use to watch a log in real time while something is actively happening on the system.

7. **wc** — counts lines, words, and bytes in a file all at once, printed as three numbers before the filename.

8. **wc -l** — narrows that down to just the line count, which is the number I actually care about most of the time.

9. **file** — looks at a file's contents (not just its extension) and tells you what type it actually is — plain text, a script, a binary, a compressed archive, etc.

10. **stat** — pulls up a file's full metadata: size, permissions, owner, and three separate timestamps (access, modify, change), plus its inode number. Way more detail than `ls -l` shows.
