# Day 07: Ownership & Special Bits
## Phase 2 - Permissions, Ownership & Security | Day 7 of 30

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
I set up a shared project folder, assigned it to a team group with `chgrp`, then applied the SGID bit so any file created inside would automatically inherit that group rather than defaulting to whoever created it. From there I ran a system-wide `find -perm /4000` sweep to see which binaries had the SUID bit set.

## What surprised me
The SUID audit turned up more binaries than I expected — programs like `passwd` and `sudo` need it to function, but it drove home why security teams treat an unexpected SUID binary as a red flag. Since SUID lets a program run with its owner's permissions rather than the caller's, one misconfigured binary is a real privilege escalation path, not just a theoretical one.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 6: Reading & Setting Permissions](../day-06-permissions/)
- Next day: [Day 8: Privilege Escalation & Identity](../day-08-privilege-escalation/)
