# Ansible Role: Docker

[![Build Status](https://travis-ci.com/herealways/ansible-role-pyenv.svg?branch=master)](https://travis-ci.com/herealways/ansible-role-pyenv)

An Ansible Role that installs [pyenv](https://github.com/pyenv/pyenv) and specified python versions using pyenv on Linux.

## Requirements

None.

## Role Variables

Variables in defaults/main.yml are listed below:

`download_cache`: boolean. If it is true, this role will download python from `python_download_url` as cache. This may be useful when the default pyenv install is very slow.

`python_download_url`: Where to download python. It is only useful when `download_cache` is true.

`python_versions`: Python versions that you want to install.

`RedHat_dependencies` and `Debian_dependencies` are dependencies for RedHat and Debian platform to build python.


## Dependencies

None

## Example Playbook
```yaml
- hosts: all
  roles: ansible-role-pyenv
```

## License

MIT

## Author Information

This role was created in 2020 by herealways.
