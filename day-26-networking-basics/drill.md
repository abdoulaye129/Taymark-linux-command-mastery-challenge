#  Day 26 drill

## Task
Identify your machine's IP address and default gateway, test connectivity to
a public host, fetch a URL's headers only, and list every port currently
listening.

## Commands run, in order

ip a
ip route
ping -c 4 8.8.8.8
curl -I https://example.com
ss -tulnp
