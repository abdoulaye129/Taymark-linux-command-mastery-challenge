#  Day 23 drill

## Task
Pick a service, stop it, confirm it is inactive, restart it, enable it to
auto-start at boot in a single combined command, and confirm both its active
and enabled state.

## Commands run, in order

sudo systemctl stop nginx
systemctl is-active nginx
sudo systemctl restart nginx
sudo systemctl enable --now nginx
systemctl is-active nginx
systemctl is-enabled nginx
