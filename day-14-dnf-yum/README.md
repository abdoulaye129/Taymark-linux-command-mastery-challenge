# Day 14: DNF/YUM & Alternative Installs
## Phase 3 - Users, Groups & Package Management | Day 14 of 30

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
On an Amazon Linux box, I ran `dnf update`, installed the same utility I'd used on Day 13 with `dnf install`, and confirmed it landed using `rpm -qa`. I then compared the whole workflow against the APT steps from yesterday to see where the two ecosystems actually differ.

## What surprised me
`dnf update` does in one step what APT splits into two (`apt update` then `apt upgrade`). It felt like a small thing, but it says something about how the two tools think about the update process differently, not just a naming difference. It's a good reminder not to assume commands map one-to-one across distributions just because the concepts are the same.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 13: APT Package Management](../day-13-apt-package-management/)
- Next day: [Day 15: Users & Packages Checkpoint](../day-15-provisioning-checkpoint/)
