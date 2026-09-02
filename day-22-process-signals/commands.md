# Day 22: Controlling Processes with Signals

1. **kill** — sends a termination signal to a process by PID. By default it's a polite request, not a punch. The process can still catch it and shut down gracefully.

2. **kill -9** — the nuclear option. No warning, no cleanup, no chance for the process to save its work. Use it when nothing else works, not as your first move.

3. **kill -HUP** — sends the "hangup" signal, which a lot of services interpret as "reload your config" instead of "die." Handy when you want a service to pick up new settings without a full restart.

4. **killall** — kills every process matching a name, not just one PID. Powerful, but dangerous if two unrelated programs happen to share a name.

5. **pkill** — similar to `killall`, but matches by pattern instead of exact name, giving you more flexibility in what gets targeted.

6. **fg** — brings a background or suspended job back to the foreground, so it's running in front of you again and taking over your terminal.

7. **bg** — resumes a suspended job, but keeps it running in the background instead of pulling it back to the front.

8. **Ctrl+Z (suspend)** — pauses a running process without killing it. The job just sits there, frozen, until you tell it to resume with `fg` or `bg`.

9. **nohup** — starts a process that ignores the hangup signal, meaning it keeps running even after you log out or close the terminal.

10. **disown** — detaches a job from your current shell, so closing the terminal won't kill it, even if you forgot to launch it with `nohup` in the first place.
