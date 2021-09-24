Ansible role: Pi-hole

[![CI](https://github.com/blalop/ansible-role-pihole/workflows/CI/badge.svg?event=push)](https://github.com/blalop/ansible-role-pihole/actions?query=workflow%3ACI)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-blalop.pihole-B62682.svg)](https://galaxy.ansible.com/blalop/pihole)

This role installs [Pi-Hole](https://pi-hole.net/) via installation script and (optionally) [eko](https://github.com/eko)'s [Pi-hole Exporter](https://github.com/eko/pihole-exporter).

Made with [Idealista's cookiecutter template](https://github.com/idealista/cookiecutter-ansible-role).

## Requirements

No special requirements. Use it in your playbook like this:

```
- hosts: all
  roles:
    - blalop.pihole
```

## Testing

Test the role via molecule:

```
pip install molecule
molecule test
```
