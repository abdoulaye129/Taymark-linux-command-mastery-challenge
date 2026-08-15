# Day 05: Paths, Links & Tree Structures
## Phase 1 - File Navigation & Filesystem Mastery | Day 5 of 30 (Checkpoint)

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
This is the Phase 1 checkpoint, so it pulls together the whole week rather than teaching something brand new. I made a symbolic link to a config file, then used `readlink` and `realpath` to trace exactly what it pointed to and where that path really resolved on disk. I finished by printing a two-level `tree` of `/etc` to see its structure without drowning in output, and talking anyone that comes across this through the difference between a hard link and a symbolic link.

## What surprised me
Explaining the hard-link-vs-symlink distinction out loud made it click harder than reading about it did. A hard link is really just another name pointing at the same data — delete the original and the data survives. A symlink is a pointer to a path, so if that path disappears, the link breaks and points at nothing.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 4: Searching the Filesystem](../day-04-filesystem-search/)
- Next day: [Day 6: Reading & Setting Permissions](../day-06-permissions/)
