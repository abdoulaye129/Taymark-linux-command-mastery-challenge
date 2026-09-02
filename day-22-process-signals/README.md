# Day 22: Controlling Processes with Signals
## Phase 5 - Process & Service Management | Day 22 of 30

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
Started a long `sleep` command, then hit Ctrl+Z to freeze it mid-run. Brought it back with `bg` instead of `fg`, so it kept running but stayed out of my way. Then I started a second one with `nohup` and `disown`, the combo that makes a process survive even after you log out.

## What surprised me
Honestly? I thought killing a process was always instant. It's not. `kill` sends a signal and politely asks the process to wind down — `kill -9` is the one that just yanks the plug, no manners involved. Big difference when you're dealing with something mid-write to a database. Skip `-9` unless you genuinely mean it.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 21: Viewing Processes](../day-21-viewing-processes/)
- Next day: [Day 23: Init Systems & systemctl Basics](../day-23-systemctl-basics/)
