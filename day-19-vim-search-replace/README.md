# Day 19: Vim Navigation & Search/Replace
## Phase 4 - Environment, Vim & Text Processing | Day 19 of 30

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
I opened a 50-line config file and jumped straight to line 10 using `:10`. No scrolling. Then I searched for a keyword with `/`, cycled through every match using `n`, and finished by replacing every instance of that word across the whole file with `:%s/old/new/g`. Closed the file with `ZZ`.

## What surprised me
Honestly, `:%s/old/new/g` did more work than I expected from one line of typing. Skip the `g` at the end, though, and Vim only replaces the first match on each line — everything else on that line gets left alone. Easy mistake. To be fair, it's the kind of thing you only really learn by getting bitten by it once.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 18: Vim Fundamentals](../day-18-vim-fundamentals/)
- Next day: [Day 20: Text Processing & Pipes](../day-20-text-processing-checkpoint/)
