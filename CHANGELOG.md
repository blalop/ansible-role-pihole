# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/) and [Keep a changelog](https://github.com/olivierlacan/keep-a-changelog).

## [Unreleased](https://github.com/blalop/ansible-role-pihole/tree/main)
* [#7](https://github.com/blalop/ansible-role-pihole/issues/7) Debian 11 support @blalop

## [1.0.1](https://github.com/blalop/ansible-role-pihole/tree/1.0.1) - 2021-07-03
### Fixed
* [#5](https://github.com/blalop/ansible-role-pihole/issues/5) When no password is provided, skip exporter parameter @blalop

## [1.0.0](https://github.com/blalop/ansible-role-pihole/tree/1.0.0) - 2021-06-30
### Added
* [#3](https://github.com/blalop/ansible-role-pihole/issues/3) Allow no password @blalop
### Breaking :warning:
* For password changing, pihole_force_reinstall has to be set to true @blalop
* No password configured by default @blalop

## [0.4.0](https://github.com/blalop/ansible-role-pihole/tree/0.4.0) - 2021-02-27
### Added
* [#1](https://github.com/blalop/ansible-role-pihole/issues/1) Support for pihole exporter @blalop

## [0.3.2](https://github.com/blalop/ansible-role-pihole/tree/0.3.2) - 2021-01-23
### Added
* Also tag installation checks @blalop

## [0.3.1](https://github.com/blalop/ansible-role-pihole/tree/0.3.1) - 2021-01-22
### Fixed
* Fixed password setting idempotence @blalop

## [0.3.0](https://github.com/blalop/ansible-role-pihole/tree/0.3.0) - 2021-01-21
### Added
* Added password setting support @blalop

## [0.2.0](https://github.com/blalop/ansible-role-pihole/tree/0.2.0) - 2021-01-16
### Added
* Use /tmp when downloading install script @blalop
* Don't copy the lighttpd conf when it's not being installed @blalop

## [0.1.0](https://github.com/blalop/ansible-role-pihole/tree/0.1.0) - 2021-01-16
### Added
* Initial release @blalop
