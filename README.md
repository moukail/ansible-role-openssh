Ansible Role OpenSSH
=========

Example Requirements
--------------------

```yml
---
roles:
  - name: ansible-role-openssl
    src: git+https://github.com/moukail/ansible-role-openssh.git
    version: main

  - name: ansible-role-openssh
    src: git+https://github.com/moukail/ansible-role-openssh.git
    version: main

```

Example Playbook
----------------

```yml
---
- name: Install OpenSSH
  hosts: all
  become: true

  vars:
    openssl_ver: "3.6.0"
    openssh_ver: "10.2p1"

  roles:
    - ansible-role-openssh

```
