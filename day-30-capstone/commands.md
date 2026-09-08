# Day 30 · Capstone: Full System Command Mastery Review

1. **Build a full system health-check script** — pulling together everything from Phase 5 and Phase 6 into one script that reports on the actual state of a server, not just one piece of it.

2. **Combine ps + systemctl + journalctl in one report** — checking process status, service status, and recent logs together, since a real health check never relies on just one signal.

3. **SSH into a remote host and run a command** — using key-based auth from Day 27 to reach a remote server and execute something there, not just locally.

4. **scp a file as part of a deployment** — pushing a file to the remote server securely, the same way I practiced on Day 27, but now as one step in a bigger flow.

5. **Apply chmod/chown to deployed files** — making sure whatever gets deployed lands with the correct permissions and ownership, back to Day 6 and Day 7.

6. **Schedule the health check with cron** — automating the whole thing to run on its own, the same pattern from Day 29, just pointed at something bigger.

7. **Parse logs with grep, awk, and sed** — pulling the pieces I actually care about out of raw log noise, back to Day 20's pipeline thinking.

8. **Use find to clean up stale files** — hunting down old files by age or size and clearing them out, straight from Day 4.

9. **Run a security audit (last, who, history)** — checking who's been on the box and what they've done, the same audit trio from Day 10.

10. **Present the 300-command journal for review** — walking a peer through the full journal and explaining any command drawn at random, cold, no notes.
