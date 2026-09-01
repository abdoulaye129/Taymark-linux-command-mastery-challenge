# Day 21: Viewing Processes
## Phase 5 - Process & Service Management | Day 21 of 30

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
I found a process by name using `pgrep`, then watched it live in `top`. From there, `pstree -p` showed me where it sat in the wider process tree — which process spawned it, basically. Last step: `lsof -i :80` to see exactly what was listening on port 80.

## What surprised me
`pstree` made something click that a flat `ps` list never quite showed me. Processes aren't just a pile of independent entries — they're a whole family tree, with parents spawning children spawning more children. Killing a parent process further up that chain can take down everything beneath it, which suddenly makes a lot more sense after seeing the structure laid out visually.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 20: Text Processing & Pipes](../day-20-text-processing-checkpoint/)
- Next day: [Day 22: Controlling Processes with Signals](../day-22-process-signals/)
