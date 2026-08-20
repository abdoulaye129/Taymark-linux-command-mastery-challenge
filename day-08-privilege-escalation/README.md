# Day 08: Privilege Escalation & Identity
## Phase 2 - Permissions, Ownership & Security | Day 8 of 30

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
I deliberately ran a command that needed root — reading `/etc/shadow` — and let it fail with a permission error. Instead of retyping it, I re-ran it with `sudo !!`, which just prefixes the previous command with `sudo`. Then I checked `sudo -l` to see the full, explicit list of what my account is actually authorised to run with elevated privileges.

## What surprised me
`sudo -l` gave a much narrower list than I assumed. I'd figured having `sudo` access meant blanket root, but it's scoped — some accounts are only permitted specific commands, not `sudo` in general. That's clearly by design: it limits the blast radius if an account gets compromised, rather than handing out all-or-nothing root.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 7: Ownership & Special Bits](../day-07-ownership/)
- Next day: [Day 9: Integrity, Encryption & Firewalling](../day-09-integrity-firewall/)
