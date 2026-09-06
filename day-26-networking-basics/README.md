# Day 26: Networking Basics
## Phase 6 - Networking, Scripting & SSH Mastery | Day 26 of 30

## Commands covered today
See [commands.md](./commands.md) for all 10, each in my own words, with a note on when I'd actually use it.

## What I practiced
Checked my IP address and default gateway with `ip a` and `ip route`, pinged a public host to confirm real connectivity, then used `curl -I` to grab just a site's headers without pulling the whole page. Closed it out listing every listening port with `ss -tulnp`.

## What surprised me
`curl -I` is such a small flag for how useful it turned out to be. I didn't need the whole page, just proof a server was actually responding and what it was sending back. Way faster than opening a browser for a quick sanity check. Also, `ss` genuinely replaced `netstat` for me today — same information, noticeably snappier.

## Evidence
Screenshot or terminal copy of the drill in [evidence/](./evidence/).

## Related
- Previous day: [Day 25: Process & Service Checkpoint](../day-25-operational-snapshot-checkpoint/)
- Next day: [Day 27: Remote Access & File Transfer](../day-27-ssh-file-transfer/)
