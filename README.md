Docker installation
=========

Ansible role for installing 'docker engine', 'docker compose', 'docker-cli' and 'containerd' on Ubuntu.

Requirements
------------

Ubuntu 22.04 with ssh access.

Role Variables
--------------

| Variable | Default | Description |
|----------|---------|-------------|
| `docker_compose_version` | `2.24.5` | Setup for docker version |
| `docker_users` | `[{{ ansible_user_id }}]` | A dictionary of docker users |

Dependencies
------------

None

Example Playbook
----------------

```yml
- hosts: vpn
  become: yes
  roles:
   - ansible-role-docker-installation
```

License
-------

MIT License

Author Information
------------------

This role was created in 2026 by [Karen Saakov](https://linkedin.com/in/karen-saakov-4905571a1) DevOps Engineer Karo LLC.
