#  Day 24: Deeper Service Management & Logs

1. **systemctl list-units --type=service** — lists every service systemd currently knows about, running or not. Good for getting a full inventory instead of checking services one by one.

2. **systemctl list-units --state=failed** — narrows that same list down to only the services that crashed or failed to start. First thing I'd run on a shaky server.

3. **systemctl daemon-reload** — tells systemd to re-read its unit files after you've edited one. Skip this and your changes just sit there, ignored.

4. **journalctl** — opens the full systemd journal, every log entry from every service, all in one place. Overwhelming without filters, so you rarely run it bare.

5. **journalctl -f** — follows the journal live, printing new entries as they happen. The `tail -f` of the systemd world.

6. **journalctl -u** — filters the journal down to logs from one specific service, cutting out all the noise from everything else.

7. **journalctl --since** — filters by time (e.g. "1 hour ago" or a specific date), so you're not scrolling through the entire journal history.

8. **journalctl -p err** — filters by priority level, showing only error-level messages and above. Skips the informational noise entirely.

9. **tail -f /var/log/syslog** — follows the classic system log file live, the old-school way of watching logs before journalctl came along.

10. **tail -f /var/log/auth.log** — same idea, but specifically for authentication events — logins, sudo usage, failed password attempts. The one I'd check first if something feels off security-wise.
