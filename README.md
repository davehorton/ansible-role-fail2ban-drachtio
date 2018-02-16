# ansible-role-fail2ban-drachtio

This is an ansible role for installing fail2ban on a [drachtio server](https://github.com/davehorton/drachtio-server).  It installs and configures fail2ban, and adds the configuration to monitor the drachtio log file for spammers.

## Role variables

The sip port(s) that drachtio is listening on
```
drachtio_ports: "5060"  # use comma-separated if multiple ports
```

## Example playbook
```
---
- hosts: all
  roles:
    - ansible-role-fail2ban-drachtio
  become: yes
```
