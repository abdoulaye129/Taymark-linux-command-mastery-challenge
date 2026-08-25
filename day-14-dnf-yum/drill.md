# drill.md — Day 14

## Task
On an Amazon Linux or RHEL box, install a package with dnf, confirm it with
rpm -qa, then compare the workflow against the equivalent apt steps from
Day 13.

## Commands run, in order

sudo dnf update
sudo dnf install tree
rpm -qa | grep tree
dnf remove tree
