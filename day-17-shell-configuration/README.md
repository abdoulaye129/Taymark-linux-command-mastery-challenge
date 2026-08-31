# Day 17: Persisting Configuration
## Phase 4 - Environment, Vim & Text Processing | Day 17 of 30

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
I added a permanent environment variable and a custom alias directly to `.bashrc`, then used `source` to reload it in my current terminal without needing to close and reopen anything. To be thorough, I also started a fresh shell afterward and confirmed both the variable and the alias were still there.

## What surprised me
`source` felt almost too simple for what it actually does — most changes to a script need a completely new process to take effect, but `source` runs the file inside your existing shell instead of a subshell, which is exactly why the changes stick around afterward. It closed the loop from yesterday: `export` alone is session-only, but writing it into `.bashrc` and sourcing it is what makes a change genuinely permanent.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 16: Environment Variables](../day-16-environment-variables/)
- Next day: [Day 18: Vim Fundamentals](../day-18-vim-fundamentals/)
