# drill.md — Day 9

## Task
Generate a SHA-256 checksum for a downloaded file to verify its integrity, make
a file immutable with chattr, then open only port 22 and port 443 on the
firewall.

## Commands run, in order

sha256sum downloaded-file.tar.gz
chattr +i important-config.conf
lsattr important-config.conf
sudo ufw allow 22
sudo ufw allow 443
sudo ufw enable
sudo ufw status
