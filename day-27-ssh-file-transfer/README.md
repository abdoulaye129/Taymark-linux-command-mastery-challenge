# Day 27: Remote Access & File Transfer
## Phase 6 - Networking, Scripting & SSH Mastery | Day 27 of 30

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
Generated a fresh keypair with `ssh-keygen`, pushed the public half over with `ssh-copy-id`, then connected to the remote host with zero password prompt. From there I moved a file up with `scp`, then pulled a different one back down, just to prove it works both directions.

## What surprised me
Connecting without typing a single password felt almost suspicious, not gonna lie. Like, it just... worked? But that's the whole point of key-based auth — the private key never leaves your machine, only the public half gets shared, and the server uses that to confirm it's really you. No password floating around to get intercepted or guessed. Genuinely changed how I think about server access after today.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 26: Networking Basics](../day-26-networking-basics/)
- Next day: [Day 28: Bash Scripting Foundations](../day-28-bash-scripting/)
