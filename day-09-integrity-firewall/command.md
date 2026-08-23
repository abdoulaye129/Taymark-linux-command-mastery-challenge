# commands.md — Day 9: Integrity, Encryption & Firewalling

1. **md5sum** — generates an MD5 checksum for a file, giving you a fingerprint you can compare against a known-good value to confirm the file wasn't altered. Fast, but considered weak for security purposes these days.

2. **sha256sum** — does the same job as `md5sum` but with a stronger, more collision-resistant algorithm. This is the one I'd actually trust when verifying a download really is what it claims to be.

3. **gpg --gen-key** — generates a new GPG keypair (public and private), which is the starting point for doing any encryption or signing with GPG.

4. **gpg --encrypt** — encrypts a file using a recipient's public key, so only the matching private key can decrypt it.

5. **gpg --decrypt** — reverses that process, decrypting a file using your own private key.

6. **chattr +i** — makes a file immutable at the filesystem level, so it can't be modified, renamed, or deleted by anyone — not even root — until the attribute is removed.

7. **lsattr** — lists the extended attributes on a file, which is how you'd check whether `chattr +i` (or another attribute) is actually set.

8. **ufw enable** — turns on the Uncomplicated Firewall, activating whatever rules are currently configured.

9. **ufw allow** — adds a rule permitting traffic on a specific port or service (e.g. `ufw allow 22`), so you open access deliberately rather than leaving everything wide open or blocking things you actually need.

10. **ufw status** — shows the firewall's current state and active rules, which is the first thing I'd check to confirm a change actually took effect.
