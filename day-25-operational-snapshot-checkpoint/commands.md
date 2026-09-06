#  Day 25 · Checkpoint: Process & Service Checkpoint

1. **ps aux | grep** — filters the full process list down to just the one you're hunting for. Simple, works everywhere, honestly still my first instinct even after learning `pgrep`.

2. **systemctl status <svc>** — the go-to for checking one specific service: running or not, recent logs, PID, all in one glance.

3. **journalctl -u <svc> --since today** — pulls today's logs for one service specifically, skipping the entire history you don't care about.

4. **kill -0 (liveness check)** — sends no actual signal, just checks whether a process with that PID still exists. A quiet way to test "is this thing even alive" without disturbing it.

5. **uptime** — shows how long the system's been running, plus the load average. One line, tells you a lot.

6. **free -h** — shows memory usage in human-readable units, total, used, and free. First thing I'd check if a server feels sluggish.

7. **vmstat** — a snapshot of memory, processes, and CPU activity, refreshed at an interval you set. Good for spotting a pattern over a few seconds instead of one frozen moment.

8. **iostat** — reports disk I/O activity, which matters when something's slow and it's not obviously CPU or memory related.

9. **watch** — reruns a given command repeatedly at a set interval, so you can watch a value change live without typing the command over and over yourself.

10. **crontab -e / crontab -l** — `-e` edits your scheduled jobs, `-l` lists what's currently scheduled. The two commands you actually need for cron.
