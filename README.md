# pip

[![Build Status](https://travis-ci.org/sysdev-samc/pip.svg?branch=master)](https://travis-ci.org/sysdev-samc/pip)

This role can be used to install pip module python for mode connected or not connected.
In this role, you have:

- pip = 9.0.1
- virtualenv = 15.1.0

SSL SNI support to Python version prior to 2.7.9

## Supports

- Debian 7,8,9
- Ubuntu 14,16,18
- Centos 7

## Role Variables

pip_config_timeout: `timeout` see manpage pip.conf

        pip_config_timeout: 60

pip_config_index_url: `index_url` Base URL of Python Package Index

        pip_config_index_url: https://pypi.python.org/simple/

## Example Playbook

        - hosts: all
          roles:
             - { role: pip }

## Test

Use `molecule` (https://molecule.readthedocs.io/en/latest) to test role

        molecule test

## License

MIT

## Author Information

Role created by dev-samc
