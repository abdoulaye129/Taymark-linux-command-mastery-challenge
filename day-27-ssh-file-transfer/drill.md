#  Day 27 drill

## Task
Generate an SSH key pair, copy the public key to a remote host, connect
without a password, then securely copy a file to and from that server.

## Commands run, in order

ssh-keygen -t ed25519
ssh-copy-id user@remotehost
ssh user@remotehost
scp localfile.txt user@remotehost:/home/user/
scp user@remotehost:/home/user/remotefile.txt ./
