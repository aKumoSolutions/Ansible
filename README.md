# Ansible

## What is Ansible?

<p align="center">
  <img width="300" height="150" src="img/Ansible.jpg">
</p>

Ansible is an open source automation platform. It's simple yet powerful. Ansible can help you with config management, deployment and task automation.

Ansible uses SSH which is assumed to be installed on all the systems you want to manage. Also it’s written in Python which needs to be installed on the remote host.

[Official Documentation](https://www.ansible.com/)

## What are Ansible ad-hoc commands?
<p align="center">
  <img width="350" height="200" src="img/adhoc.png">
</p>

Ad-hoc commands in Ansible allow you to execute simple tasks at the command line against one or all of your hosts. An ad-hoc command consists of two parameters; the host group that defines on what machines to run the task against and the Ansible module to run.

[Official Documentation](https://docs.ansible.com/ansible/latest/user_guide/intro_adhoc.html)

#### [Ad-hoc Commands - Examples](ad-hoc)
## What are Ansible Playbooks?
<p align="center">
  <img width="250" height="150" src="img/AnsiblePlaybook.png">
</p>

Ansible playbooks are highly customizable scripts that are used to execute a series of tasks and commands. 

A playbook is like a recipe or an instructions manual which tells Ansible what to do when it connects to each machine. Playbooks are written in YAML

## [Playbooks](playbooks)

| Playbook | Description |
| -------- | ----------- |
| [ping.yaml](playbooks/ping.yaml) | Simple Ansible playbook to ping all hosts. | 
| [install_vim.yaml](playbooks/install_vim.yaml) | Ansible playbook - installs ```vim```, if the Linux distribution is CentOS7. |
| [multi_users.yaml](playbooks/multi_users.yaml)  | Ansible playbook - adds multiple users to all managed hosts. |
| [update-reboot.yaml](playbooks/update-reboot.yaml) |Ansible playbook - update packages in Linux (CentOS, Debian, Ubuntu, Fedora, Amazon-Linux. Suse) and reboots the system. |
| [ubuntu_debian_kernel_patch.yaml](playbooks/ubuntu_debian_kernel_patch.yaml) | Ansible playbook - downloads, updates kernel and packages in Ubuntu and reboots the system. |
| [500Mlogfile.yaml](playbooks/500Mlogfile.yaml) | Ansible playbook - creates a logfile under tmp folder, size=500M. |
| [archive_log_file.yaml](playbooks/archive_log_file.yaml) | Ansible playbook - archives log files, size < 50M. |
| [fail2ban.yaml](playbooks/archive_log_file.yaml) | Ansible playbook - installs ```fail2ban``` on Redhat/CentOS 6 & 7. |
| [lineinfile.yaml](playbooks/lineinfile.yaml) | Ansible playbook - change a line in a file. |
| [ssh_port_change.yaml](playbooks/ssh_port_change.yaml) | Ansible playbook - change ```ssh``` port. |
| [wordpress.yaml](playbooks/wordpress.yaml) | Ansible playbook - installs ```wordpress``` on Redhat/CentOS 7. |
| [atop_installation.yaml](playbooks/atop_installation.yaml) | Ansible playbook - installs ```atop``` on Redhat/CentOS 7. |