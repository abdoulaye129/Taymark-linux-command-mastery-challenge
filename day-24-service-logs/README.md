# Day 24: Deeper Service Management & Logs
## Phase 5 - Process & Service Management | Day 24 of 30

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
Ran `systemctl list-units --state=failed` first, just to see if anything was quietly broken on the box. Nothing was, thankfully. Then I pulled today's logs for nginx specifically, filtered down to error-level only with `journalctl -u nginx --since today -p err`, and finished by watching it live for a minute with `-f`.

## What surprised me
Stacking those journalctl flags together felt like magic, not gonna lie. One command, three filters, and I went from "every log ever written on this system" down to "just today, just this service, just the errors." That's the whole game with journalctl — it's not about memorizing one command, it's about knowing which flags stack together to get you exactly what you need.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 23: Init Systems & systemctl Basics](../day-23-systemctl-basics/)
- Next day: [Day 25: Process & Service Checkpoint](../day-25-operational-snapshot-checkpoint/)
