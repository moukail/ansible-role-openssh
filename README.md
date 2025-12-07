### Ansible Role OpenSSH
```yml
---
- name: Install OpenSSH
  hosts: all
  become: true

  vars:
    openssl_ver: "3.6.0"

  roles:
    - ansible-role-openssh

```