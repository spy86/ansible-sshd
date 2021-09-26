Role Name
=========

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Provision our SSH Server.

Requirements
------------

None

Role Variables
--------------

None

Dependencies
------------

None.

Example Playbook
----------------

```YAML
---
- hosts: all
  tasks:
    - name: Template a file to /etc/ssh/sshd_config
      template:
      src: /templates/sshd_config.j2
      dest: /etc/ssh/sshd_config
      owner: root
      group: root
      mode: '0644'
```
