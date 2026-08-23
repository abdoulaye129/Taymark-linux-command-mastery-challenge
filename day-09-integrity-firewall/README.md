# Day 09: Integrity, Encryption & Firewalling
## Phase 2 - Permissions, Ownership & Security | Day 9 of 30

## Commands covered today
The full list of 10 commands is in [commands.md](./commands.md), each written in my own words along with notes on when I'd actually reach for it.

## What I practiced
I generated a SHA-256 checksum for a downloaded file to confirm it hadn't been tampered with or corrupted in transit, then used `chattr +i` to make a config file immutable and checked it with `lsattr`. To close things out, I opened only ports 22 and 443 on the firewall with `ufw allow`, then enabled it and confirmed the rules with `ufw status`.

## What surprised me
`chattr +i` was the standout for me — it locks a file down so completely that even root can't touch it until the immutable flag is removed first. Permissions like `chmod` still bend to root, but this is a separate, stricter layer underneath that. I hadn't realized there was a mechanism that bypasses root entirely.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 8: Privilege Escalation & Identity](../day-08-privilege-escalation/)
- Next day: [Day 10: Security Checkpoint & Audit](../day-10-security-audit-checkpoint/)
