#  Day 26: Networking Basics

1. **ip a** — shows every network interface on the machine along with its assigned IP address. The modern replacement for the older `ifconfig`.

2. **ip route** — shows the routing table, which includes the default gateway — basically, where traffic goes when it doesn't have a more specific route.

3. **ping -c** — sends a limited number of ICMP packets to test connectivity to a host. The `-c` flag caps how many, so it doesn't ping forever.

4. **curl** — fetches a URL from the command line and dumps the response. Simple, but ridiculously versatile once you learn its flags.

5. **curl -I** — fetches only the response headers, skipping the actual body. Quick way to check if a site's up without pulling the whole page.

6. **wget** — downloads a file from a URL straight to disk. Where `curl` prints to your terminal by default, `wget` is built for saving files.

7. **netstat -tulnp** — lists listening ports along with the process using each one. Older tool, still shows up on plenty of systems.

8. **ss -tulnp** — does the same job as `netstat -tulnp`, just faster and more modern. Most current distros lean on this one now.

9. **hostname** — prints the machine's hostname. Simple, one job, does it well.

10. **hostnamectl** — shows a fuller breakdown: hostname, OS, kernel version, architecture. `hostname` on steroids, basically.
