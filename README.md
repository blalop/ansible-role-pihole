# Pihole Ansible role

[![Build Status](https://travis-ci.com/blalop/pihole_role.svg?branch=main)](https://travis-ci.com/blalop/pihole_role)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-blalop.pihole_role-B62682.svg)](https://galaxy.ansible.com/blalop/pihole_role)

This role installs [Pi-Hole](https://pi-hole.net/) via installation script and (optionally) [eko](https://github.com/eko)'s [Pi-hole Exporter](https://github.com/eko/pihole-exporter).

Made with [Idealista's cookiecutter template](https://github.com/idealista/cookiecutter-ansible-role).

## Requirements

No special requirements. Use it in your playbook like this:

```
- name: Configure services
  hosts: pi
  tags: services
  roles:
    - role: pihole
      tags: pihole
```

## Testing

Test the role via molecule:

```
pipenv sync
pipenv run molecule test
```

## Built with

![Ansible](https://img.shields.io/badge/ansible-2.9.16-green.svg)
![Molecule](https://img.shields.io/badge/molecule-3.2.2-green.svg)
![Goss](https://img.shields.io/badge/goss-0.3.16-green.svg)
