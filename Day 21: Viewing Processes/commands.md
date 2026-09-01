# Day 21: Viewing Processes

1. **ps aux** — snapshots every running process on the system, showing user, CPU, memory, and more, all in one static list.

2. **ps -ef** — a slightly different formatting of the same idea, showing full command lines and parent process IDs. Some admins prefer this style over `aux`.

3. **ps -u** — narrows the process list down to just the ones owned by a specific user, which cuts the noise on a shared system.

4. **top** — shows a live, constantly refreshing view of running processes, sorted by resource usage by default. Good for watching what's happening right now.

5. **htop** — a more visual, interactive version of `top`, with color-coded bars and easier navigation. Not installed by default everywhere, but worth grabbing.

6. **pgrep** — searches running processes by name and returns their process IDs, without needing to eyeball a full `ps` list.

7. **pstree** — displays processes as a tree, showing which processes spawned which. Useful for understanding parent-child relationships at a glance.

8. **lsof -i** — lists open network connections and which process owns each one. This is the one I'd reach for to answer "what's using this port?"

9. **jobs** — lists background and suspended jobs tied to your current shell session specifically, not the whole system.

10. **nice / renice** — `nice` sets a process's scheduling priority when you first launch it; `renice` adjusts that priority on a process that's already running.
