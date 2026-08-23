# Day 10: Security Checkpoint & Audit
## Phase 2 - Permissions, Ownership & Security | Day 10 of 30 (Checkpoint)

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
This was the Phase 2 checkpoint, so it pulled together everything from the week into one mini audit rather than teaching something new. I used `last` to see recent login activity, `w` to see who was on the system right now, `lastlog` to spot any account that had never logged in at all, and `history | grep sudo` to review every elevated command run in the session.

## What surprised me
Running all four side by side made it obvious how much they complement each other rather than overlap. `last` tells a story over time, `w` is a live snapshot, `lastlog` is really about spotting dormant or unused accounts, and the `history` grep is the only one that shows intent — what someone actually did with their access, not just when they showed up.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 9: Integrity, Encryption & Firewalling](../day-09-integrity-firewall/)
- Next day: [Day 11: Creating & Managing Users](../day-11-user-management/)
