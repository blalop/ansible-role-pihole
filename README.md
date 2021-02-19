# Pihole Ansible role

[![Build Status](https://travis-ci.com/blalop/pihole_role.svg?branch=main)](https://travis-ci.com/blalop/pihole_role)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-blalop.pihole_role-B62682.svg)](https://galaxy.ansible.com/blalop/pihole_role)

This role installs pihole via installation script. Tested on Debian && Raspbian.

## Requirements

No special requirements.


## Role vars

| Variable                   | Default     | Additional comments                                                                                  |
| :---                       | :---        | :---                                                                                                 |
| `pihole_required_packages` | [procps]    |                                                                                                      |
| `pihole_password`          | pihole      | Pihole web interface password                                                                        |
| `pihole_force_reinstall`   | false       | Forces reinstallation                                                                                |
| `pihole_lighttpd_port`     | 80          | Web interface port                                                                                   |
| `pihole_interface`         | eth0        | [Pihole setup vars](https://discourse.pi-hole.net/t/what-is-setupvars-conf-and-how-do-i-use-it/3533) |
| `pihole_ipv4_address`      | 0.0.0.0     | [Pihole setup vars](https://discourse.pi-hole.net/t/what-is-setupvars-conf-and-how-do-i-use-it/3533) |
| `pihole_ipv6_address`      | 0:0:0:0:0:0 | [Pihole setup vars](https://discourse.pi-hole.net/t/what-is-setupvars-conf-and-how-do-i-use-it/3533) |
| `pihole_dns_1`             | 8.8.8.8     | [Pihole setup vars](https://discourse.pi-hole.net/t/what-is-setupvars-conf-and-how-do-i-use-it/3533) |
| `pihole_dns_2`             | 4.4.4.4     | [Pihole setup vars](https://discourse.pi-hole.net/t/what-is-setupvars-conf-and-how-do-i-use-it/3533) |
| `pihole_query_logging`     | true        | [Pihole setup vars](https://discourse.pi-hole.net/t/what-is-setupvars-conf-and-how-do-i-use-it/3533) |
| `pihole_web_server`        | true        | [Pihole setup vars](https://discourse.pi-hole.net/t/what-is-setupvars-conf-and-how-do-i-use-it/3533) |
| `pihole_web_interface`     | true        | [Pihole setup vars](https://discourse.pi-hole.net/t/what-is-setupvars-conf-and-how-do-i-use-it/3533) |
| `pihole_lighttpd_enabled`  | true        | [Pihole setup vars](https://discourse.pi-hole.net/t/what-is-setupvars-conf-and-how-do-i-use-it/3533) |


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
