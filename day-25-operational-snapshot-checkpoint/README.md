# Day 25: Process & Service Checkpoint
## Phase 5 - Process & Service Management | Day 25 of 30 (Checkpoint)

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
This was the Phase 5 checkpoint, so it was about pulling everything from the week into one operational snapshot rather than learning anything new. Checked `uptime` first, then `free -h` for memory, then ran `systemctl status` against three key services one after another, and closed it out checking scheduled jobs with `crontab -l`.

## What surprised me
Doing this whole thing manually made me appreciate why real monitoring dashboards exist in the first place. Six commands, run one at a time, just to get a snapshot that a proper tool would show me in one screen automatically. Not complaining though — running it by hand is exactly how the pieces actually stuck this week, instead of just clicking through a dashboard without understanding what it's pulling from underneath.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 24: Deeper Service Management & Logs](../day-24-service-logs/)
- Next day: [Day 26: Networking Basics](../day-26-networking-basics/)
