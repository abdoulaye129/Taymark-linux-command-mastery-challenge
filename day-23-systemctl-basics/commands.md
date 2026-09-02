#  Day 23: Init Systems & systemctl Basics

1. **systemctl start** — kicks off a service right now. Doesn't touch whether it starts on boot, just gets it running immediately.

2. **systemctl stop** — shuts a service down right now. Same deal, boot behavior untouched.

3. **systemctl restart** — stops then starts a service in one motion. Handy after a config change that a plain reload can't handle.

4. **systemctl reload** — asks a service to re-read its config without a full stop/start. Not every service supports this — some just don't listen.

5. **systemctl enable** — sets a service to start automatically on boot. It won't start it now, just queues it for next time.

6. **systemctl disable** — removes a service from the boot startup list, so it won't launch automatically anymore.

7. **systemctl enable --now** — the shortcut version. Enables for boot and starts it immediately, both in one line instead of two commands.

8. **systemctl status** — shows whether a service is running, its recent logs, and its PID, all in one readable dump. My first stop when something's misbehaving.

9. **systemctl is-active** — a quick yes/no check on whether a service is currently running, without the full status output.

10. **systemctl is-enabled** — same idea, but for boot behavior instead of current state. Tells you if a service will auto-start next boot.
