# Day 03: Reading & Inspecting Files
## Phase 1 - File Navigation & Filesystem Mastery | Day 3 of 30

## Commands covered today
The full list of 10 commands lives in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
For today's drill, I picked a log file on the system and put it through its paces: viewed it in full with `cat`, paged through it with `less`, pulled the first and last 15 lines, counted its lines, checked its file type with `file`, and dug into its metadata with `stat`.

## What surprised me
I hadn't realized just how much faster `less` is than `cat` on large files since it only loads what's on screen, it doesn't have to read the whole thing first. `stat` was another surprise: it exposes access time, modify time, change time, and inode number, which is a lot more than `ls -l` ever shows you.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 2: Creating, Copying, Moving, Deleting](../day-02-file-operations/)
- Next day: [Day 4: Searching the Filesystem](../day-04-filesystem-search/)
