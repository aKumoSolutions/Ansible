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

## What are Ansible Playbooks?
<p align="center">
  <img width="250" height="150" src="img/AnsiblePlaybook.png">
</p>

Ansible playbooks are highly customizable scripts that are used to execute a series of tasks and commands. 

A playbook is like a recipe or an instructions manual which tells Ansible what to do when it connects to each machine. Playbooks are written in YAML

## [Ad-hoc Commands](ad-hoc)


## [Playbooks](playbooks)

| Playbook | Description |
| -------- | ----------- |
| [ping.yaml](playbooks/ping.yaml) | Simple Ansible playbook to ping all hosts. | 
| [install-vim.yaml](playbooks/install-vim.yaml) | Ansible playbook which installs ```vim```, if the Linux distribution is CentOS7. |
| [multipleusers.yaml](playbooks/multipleusers.yaml)  | Ansible playbook that adds multiple users to all managed hosts. |
| [update-reboot.yaml](playbooks/update-reboot.yaml) |Ansible playbook that update packages in Linux (CentOS, Debian, Ubuntu, Fedora, Amazon-Linux. Suse) and reboots the system. |
| [ubuntu_debian_kernel_patch.yaml](playbooks/ubuntu_debian_kernel_patch.yaml) | Ansible playbook that downloads, updates kernel and packages in Ubuntu and reboots the system. |