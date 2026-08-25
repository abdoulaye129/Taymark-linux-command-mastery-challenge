# Day 13: APT Package Management (Debian/Ubuntu)
## Phase 3 - Users, Groups & Package Management | Day 13 of 30

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
I refreshed the package index with `apt update`, searched for a small utility with `apt search`, installed it, then checked its details with `apt show` before removing it completely with `apt purge`.

## What surprised me
I hadn't clocked the real difference between `apt remove` and `apt purge` before today. `remove` leaves configuration files behind on purpose, so a reinstall later picks up right where you left off — it's `purge` that actually wipes the config too. Small distinction, but it explains why a "removed" package can sometimes still leave files sitting around.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 12: Groups & Access Circles](../day-12-groups/)
- Next day: [Day 14: DNF/YUM & Alternative Installs](../day-14-dnf-yum/)
