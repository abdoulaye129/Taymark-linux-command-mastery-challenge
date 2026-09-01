# Day 20: Text Processing & Pipes
## Phase 4 - Environment, Vim & Text Processing | Day 20 of 30 (Checkpoint)

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
This was the Phase 4 checkpoint, so instead of new commands it was about chaining what I already knew into one working pipeline. I filtered a raw log for "error" entries with `grep -i`, pulled just the timestamp columns with `awk`, then piped that into `sort` and finally `uniq` to strip out duplicates. One line, four tools, each one feeding the next.

## What surprised me
`uniq` only catches duplicates that are sitting right next to each other. Miss the `sort` step beforehand, and identical lines scattered throughout the file just slide right past it. That's honestly the whole point of a pipeline, though — each tool does one small job well, and the order you chain them in matters just as much as which tools you pick.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 19: Vim Navigation & Search/Replace](../day-19-vim-search-replace/)
- Next day: [Day 21: Viewing Processes](../day-21-viewing-processes/)
