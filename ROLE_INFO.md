ansible-role-yay
=========

Install YAY on Arch and any packages through a single role

Requirements
------------
N/A

Role Variables
--------------

```yaml
---
# defaults file for ansible-role-yay
ansible_arch_yay:
  # The yay git source repository
  git: "https://aur.archlinux.org/yay.git"
  # The owner of the repository
  owner:
    name: "{{ user }}"
    group: "{{ user }}"
  
  # Destination to clone yay to
  dest: "/home/{{ user }}/yay"

yay_role_apps: 
```

Dependencies
------------

N/A

Example Playbook
----------------
```yaml
    - hosts: servers
      roles:
         - { role: ansible-role-yay}
```
License
-------

GPLv3

Author Information
------------------

John Stilia - stilia.johny@gmail.com

