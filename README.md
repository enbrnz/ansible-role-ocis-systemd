# ansible-role-ocis-systemd
Simple ansible role to install ownCloud infinite scale as systemd service

---
## What it does
1. Create a group
2. Create a system_user in group, Shell: /sbin/nologin, Home: /var/lib/ocis 
3. Create /etc/ocis with ownership system_user:group
4. Create /etc/ocis/ocis.env
5. Create a random ocis admin password
6. Run ocis init
7. Create a systemd unit file
8. Enable and start systemd unit
