# Day 15: Users & Packages Checkpoint
## Phase 3 - Users, Groups & Package Management | Day 15 of 30 (Checkpoint)

## Commands covered today
The full list of 10 commands lives in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
This was the Phase 3 checkpoint, so it combined user provisioning and package management into one realistic task instead of introducing anything new. I created a new account with a home directory and multiple group memberships in a single `useradd -m -G` command, set its password, confirmed the identity with `id`, then installed the three tools that account would need with a chained `apt update && apt install -y`. I closed out by checking the installs with `dpkg -l | grep` and reviewing the session with `history`.

## What surprised me
Doing the whole provisioning flow as one documented sequence made me realize how much of this week was really about combining commands rather than learning them in isolation — `useradd -m -G` alone replaced what would've been three separate steps back on Day 11. Chaining `apt update` and `apt install -y` with `&&` was the same idea: it's not new syntax, just a cleaner way to run steps that always belong together anyway.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 14: DNF/YUM & Alternative Installs](../day-14-dnf-yum/)
- Next day: [Day 16: Environment Variables](../day-16-environment-variables/)
