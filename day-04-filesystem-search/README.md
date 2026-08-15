# Day 04: Searching the Filesystem
## Phase 1 - File Navigation & Filesystem Mastery | Day 4 of 30

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
Today's drill was about hunting things down rather than just reading them. I searched `/etc` for every `.conf` file with `find -name`, then combed `/var` for anything over 1MB using `find -size`. From there I checked how much space `/home` was actually using with `du -sh`, and finished by checking how much room was left on the root filesystem with `df -h`.

## What surprised me
I expected `find` to be quick, but on a directory as large as `/var` it noticeably slower than `locate` would have been — because it's walking the live filesystem instead of reading a prebuilt index. That's the tradeoff: `find` is always accurate, `locate` is fast but only as current as its last `updatedb` run.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 3: Reading & Inspecting Files](../day-03-file-inspection/)
- Next day: [Day 5: Paths, Links & Tree Structures](../day-05-links-checkpoint/)
