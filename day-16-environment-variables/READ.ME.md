# Day 16: Environment Variables
## Phase 4 - Environment, Vim & Text Processing | Day 16 of 30

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
I set a temporary variable with `export`, confirmed it with `echo $TESTVAR`, then removed it with `unset` and checked it was really gone. From there I built a tiny script, added its folder to `PATH` for the current session only, and confirmed the shell could find and run it just by name, without needing the full path.

## What surprised me
Adding a directory to `PATH` this way only lasts for the current session — closing the terminal wipes it, since I never wrote it anywhere persistent. It's a good reminder that `export` on its own is temporary by nature; making a change stick for good needs to happen somewhere like `.bashrc`, which is exactly what tomorrow's topic is.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 15: Users & Packages Checkpoint](../day-15-provisioning-checkpoint/)
- Next day: [Day 17: Persisting Configuration](../day-17-shell-configuration/)