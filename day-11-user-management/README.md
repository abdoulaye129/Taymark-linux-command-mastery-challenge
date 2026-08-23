# Day 11: Creating & Managing Users
## Phase 3 - Users, Groups & Package Management | Day 11 of 30

## Commands covered today
The full list of 10 commands lives in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
I created a full user account from scratch with `useradd -m -s`, giving it a home directory and Bash shell in one step, then set a password for it. From there I added it to a secondary group with `usermod -aG`, renamed the account with `usermod -l`, and finally removed it entirely — home directory included — with `userdel -r`.

## What surprised me
The `-a` flag on `usermod -aG` matters more than I expected. Leaving it off doesn't add a group, it replaces the user's entire group list with just the one specified, silently dropping every other group they were in. That's an easy way to break someone's access without meaning to, so I'll be double-checking that flag every time from now on.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 10: Security Checkpoint & Audit](../day-10-security-audit-checkpoint/)
- Next day: [Day 12: Groups & Access Circles](../day-12-groups/)
