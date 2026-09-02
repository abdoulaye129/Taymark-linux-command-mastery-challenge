# Day 23: Init Systems & systemctl Basics
## Phase 5 - Process & Service Management | Day 23 of 30

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
Stopped nginx cold, confirmed it was down with `is-active`, then restarted it and enabled it for boot — all with `enable --now` doing both jobs in one line. Closed it out by checking both `is-active` and `is-enabled` separately, just to be sure the two states actually matched what I expected.

## What surprised me
"Running" and "will start on boot" are two completely separate settings. I assumed they moved together — start a service, it's obviously enabled, right? Wrong. You can have a service running right now that won't come back after a reboot, and one that's enabled for boot but sitting dead right this second. Two different knobs, not one.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 22: Controlling Processes with Signals](../day-22-process-signals/)
- Next day: [Day 24: Deeper Service Management & Logs](../day-24-service-logs/)
