# Day 28: Bash Scripting Foundations
## Phase 6 - Networking, Scripting & SSH Mastery | Day 28 of 30

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
Wrote a script from scratch — shebang, `chmod +x`, the whole setup. It asked for my name, checked whether a config file existed using an `if` statement, then looped through three server names, pinging each one in turn with a `for` loop.

## What surprised me
Forgot the space around my `if` brackets on the first try and the whole thing just refused to run, no helpful error, nothing. Bash is genuinely unforgiving about spacing in ways most languages aren't. Also realized `for server in server1 server2 server3` is basically the same shape as every day-2 drill I've been doing manually all month — it's just automating what I'd have typed by hand three separate times.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 27: Remote Access & File Transfer](../day-27-ssh-file-transfer/)
- Next day: [Day 29: Functions, Arguments & Automation](../day-29-functions-automation/)
