Ansible Role: osx-command-line-tools
====================================

[![Galaxy Role][badge-role]][link-galaxy]
[![Downloads][badge-downloads]][link-galaxy]
[![MIT Licensed][badge-license]][link-license]
[![Build Status][badge-travis]][link-travis]
[![Requirements Status][badge-requires]][link-requires]

An Ansible role that installs OS X Command Line Tools.

Requirements
------------

None (except running on Mac OS X).

Role Variables
--------------

Going forward, all role variables will be prefixed with `clt_` (for **C**ommand
**L**ine **T**ools) to avoid ambiguity and namespace collision.

| Variable Name                        | Description                                                               | Default |
| :---                                 | :---                                                                      |  :---:  |
| `clt_force_install`                  | Install the Command Line Tools, even if already installed                 |  `no`   |
| `clt_softwareupdate_list_timeout`    | How long (in seconds) to wait for an available Command Line Tools package |  `300`  |
| `clt_softwareupdate_install_timeout` | How long (in seconds) to wait for installation of the Command Line Tools  |  `1200` |

Dependencies
------------

None.

Example Playbook
----------------

A simple playbook example:

    - hosts: servers
      roles:
         - { role: elliotweiser.osx-command-line-tools }


License
-------

[MIT][link-license]

Contributing
------------

Please read the [contributing guidelines](CONTRIBUTING.md).

Author Information
------------------

[Elliot Weiser](https://github.com/elliotweiser)

[badge-downloads]: https://img.shields.io/ansible/role/d/14481.svg?style=flat-square
[badge-license]: https://img.shields.io/github/license/elliotweiser/ansible-osx-command-line-tools.svg?style=flat-square
[badge-requires]: https://img.shields.io/requires/github/elliotweiser/ansible-osx-command-line-tools.svg?style=flat-square
[badge-role]: https://img.shields.io/ansible/role/14481.svg?style=flat-square
[badge-travis]: https://img.shields.io/travis/elliotweiser/ansible-osx-command-line-tools/master.svg?style=flat-square
[link-galaxy]: https://galaxy.ansible.com/elliotweiser/osx-command-line-tools/
[link-license]: https://raw.githubusercontent.com/elliotweiser/ansible-osx-command-line-tools/master/LICENSE
[link-requires]: https://requires.io/github/elliotweiser/ansible-osx-command-line-tools/requirements/?branch=master
[link-travis]: https://travis-ci.org/elliotweiser/ansible-osx-command-line-tools
