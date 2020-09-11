## Ansible ad-hoc commands syntax

<p align="center">
  <img width="650" height="150" src="../img/adhocsyntax.png">
</p>

### Ping all managed hosts
```
ansible all -m ping
```

### Check free memory of all managed hosts
```
ansible all -a "free -m"
```
OR
```
ansible all -m shell -a "free -m"
```

### Check uptime of all managed hosts
```
ansible all -a uptime
ansible all -m command -a uptime
ansible all -m shell -a uptime
```

### Check disk space of all managed hosts
```
ansible all -a "df -h"
ansible all -m shell -a "df -h"
ansible all -m command -a "df -h"
```
