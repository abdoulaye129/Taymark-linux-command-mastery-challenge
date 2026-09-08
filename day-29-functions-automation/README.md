# Day 29: Functions, Arguments & Automation
## Phase 6 - Networking, Scripting & SSH Mastery | Day 29 of 30

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
Rebuilt yesterday's script into a proper function that takes a service name as an argument instead of having it hardcoded. It checks the service's status, restarts it if it's down, and logs the outcome with `logger`. Scheduled the whole thing to run every hour using `crontab -e`.

## What surprised me
Wrapping the logic in a function made it instantly reusable — pass a different service name as `$1` and the exact same code just works on nginx, ssh, whatever. Didn't have to rewrite a single line. That's genuinely the whole value of a function, I just hadn't felt it in my hands until today. Also, `logger` writing straight into the system log means this thing now leaves a paper trail I can actually check later, instead of just silently doing its job in the dark.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 28: Bash Scripting Foundations](../day-28-bash-scripting/)
- Next day: [Day 30: Capstone](../day-30-capstone/)
