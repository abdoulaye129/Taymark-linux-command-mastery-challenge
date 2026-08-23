# Day 12: Groups & Access Circles
## Phase 3 - Users, Groups & Package Management | Day 12 of 30

## Commands covered today
The full list of 10 commands lives in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
I created a group called `devs`, added two users to it with `gpasswd -a`, and confirmed the membership with `getent group`. From there I removed one member with `gpasswd -d`, checked the entry again to confirm the change, and finished by deleting the group entirely with `groupdel`.

## What surprised me
Deleting the group didn't touch either user account at all — both accounts were still fully intact afterward, just no longer members of a group that no longer existed. I'd half expected some warning or side effect, but group and user management turned out to be genuinely independent of each other.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 11: Creating & Managing Users](../day-11-user-management/)
- Next day: [Day 13: APT Package Management](../day-13-apt-package-management/)
