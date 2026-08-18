# Day 06: Reading & Setting Permissions
## Phase 2 - Permissions, Ownership & Security | Day 6 of 30

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
I created a script file and set it to `rwxr-xr-x` three separate ways: first with relative `chmod +x`, then with an explicit assignment (`u=rwx,g=rx,o=rx`), and finally with the octal shorthand `chmod 755`. I ran `ls -l` after each change to confirm the permission string came out the same regardless of which method got me there.

## What surprised me
All three methods landed on the exact same permission string, but they don't behave the same way in every situation. The relative method only touches the bits you name and leaves everything else alone, while the assignment and octal methods overwrite the whole permission set outright. That distinction matters a lot more once you're scripting changes instead of doing them one file at a time.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 5: Paths, Links & Tree Structures](../day-05-links-checkpoint/)
- Next day: [Day 7: Ownership & Special Bits](../day-07-ownership/)
