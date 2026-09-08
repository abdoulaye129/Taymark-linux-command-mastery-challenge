# Day 30: Capstone — Full System Command Mastery Review
## Phase 6 - Networking, Scripting & SSH Mastery | Day 30 of 30 (Capstone)

## Commands covered today
See [commands.md](./commands.md) for the full capstone task breakdown — no new commands today, just everything from the last 29 days working together.

## What I practiced
Built one script that ties the whole challenge together. It connects to a remote server over SSH using the key-based auth from Day 27, deploys a config file with `scp`, sets the correct ownership and permissions the way I did back on Day 6 and Day 7, restarts the service, then checks it's actually healthy using `systemctl` and `journalctl`. Every step logs itself with `logger`, and the whole thing runs on a cron schedule from Day 29. Then I walked a peer through it line by line, no notes, explaining every command as we went.

## What surprised me
Nothing in this script was new. Not one command. What hit me is that thirty days ago, deploying and verifying a service change like this would've taken me a scattered afternoon of googling and guessing. Today it's fourteen lines I wrote from memory. That's genuinely the whole point of this challenge — not memorizing 300 commands as trivia, but reaching the point where they're already in your fingers when a real task shows up.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 29: Functions, Arguments & Automation](../day-29-functions-automation/)
- Next day: Challenge complete. 🎉
