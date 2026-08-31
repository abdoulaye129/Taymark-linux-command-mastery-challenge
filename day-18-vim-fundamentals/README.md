# Day 18: Vim Fundamentals
## Phase 4 - Environment, Vim & Text Processing | Day 18 of 30

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
I opened a new file in Vim, switched into insert mode to type three lines, saved and quit, then reopened the same file. From there I deleted the middle line with `dd`, immediately undid that deletion with `u` to bring it back, and saved and quit again to finish.

## What surprised me
The constant mode-switching was the real adjustment — I kept trying to type text without hitting `i` first, forgetting that Vim's default mode treats every keystroke as a command, not text. `dd` doubling as a copy was the other surprise: deleting a line doesn't just remove it, it also stores it, so a `p` right after would have pasted the exact line I'd just deleted.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 17: Persisting Configuration](../day-17-shell-configuration/)
- Next day: [Day 19: Vim Navigation & Search/Replace](../day-19-vim-search-replace/)
