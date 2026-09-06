#  Day 27: Remote Access & File Transfer

1. **ssh** — connects to a remote machine over a secure, encrypted channel. This is the backbone command for anything remote in this phase.

2. **ssh -p** — connects to a non-default port instead of the standard port 22. Common when a server's been hardened to run SSH somewhere less obvious.

3. **ssh -i** — points SSH to a specific private key file rather than relying on whatever's default. Useful when you're juggling multiple keys for different servers.

4. **ssh-keygen** — generates a new public/private keypair. The starting point for password-less, key-based authentication.

5. **ssh-copy-id** — pushes your public key to a remote server's authorized_keys file automatically, so you don't have to copy-paste it by hand.

6. **scp** — securely copies a file between local and remote machines, over the same encrypted connection SSH uses. Quick, one-off transfers live here.

7. **sftp** — an interactive, secure file transfer session, more like an FTP client but encrypted. Good when you need to browse around a remote filesystem, not just grab one file.

8. **rsync** — syncs files between locations efficiently, only transferring what's actually changed instead of copying everything from scratch every time.

9. **~/.ssh/config** — a personal config file where you can save shortcuts for servers you connect to often, so you type `ssh myserver` instead of the full username, host, and key path every time.

10. **sshd_config hardening** — the server-side config that controls how SSH itself behaves — disabling password login, restricting root login, that kind of thing. This is where real security lives.
