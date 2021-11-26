ansible_role_manage_yum_dnf
=========


[![CI](https://github.com/habbis/ansible_role_manage_yum_dnf/workflows/CI/badge.svg)](https://github.com/habbis/ansible_role_manage_yum_dnf/actions?query=workflow%3ACI)

This role manages yum and dnf config. 

Example site.yml

```
---
- name: setup puppet agent
  gather_facts: yes
  remote_user: root
  #remote_user: ansible
  #become: yes
  #become_method: sudo
  hosts: test
  #hosts: puppet-clients
  #hosts: all
  vars_files:
    -  defaults/main.yml
    #-  defaults/secrets.yml

  roles:
    - { role: ../ansible_role_manage_yum_dnf }
```
