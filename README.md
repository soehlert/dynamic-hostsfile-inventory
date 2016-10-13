# Dynamic Hosts File Inventory
Dynamic inventory for ansible from /etc/hosts (or /etc/hosts formatted) file

# Config

Copy example.conf to somewhere (default location the script will look at is ~/.config/dhfi/dhfi.conf)
Edit the file to suit your needs

```
[files]
# The file you want to read from (default is /etc/hosts)
hosts_file = /etc/hosts
# The file you want to write to (aka your ansible inventory file)
inventory = /Users/soehlert/projects/ansible/inventory

[ssh]
# The dnsmasq server you want to grab the info from
server = 10.0.0.2
# The port to ssh over (default is 22)
port = 22
# The user you want to ssh as (keep in mind file permissions on the remote end)
user = soehlert
# Defaults to using a keyfile for ssh
ssh_key = /Users/soehlert/.ssh/id_rsa
```
