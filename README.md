# Ansible role for nginx


## Tested On

  * Ubuntu 14.04

## Defaults

The `defaults/main.yml` should be pretty clear on the usage and values. The 
version used by defaults are:

  * `nginx_user`: www-data

## Usage

The tests in the respository should be pretty straight forward, but here are
some examples:

### nginx

playbook.yml:

```
- name: Install and run nginx 
  hosts: all
  sudo: True

  roles:
    - { role: ansible-nginx }

```

## TODO

  * Extract supervisor to it's own role
  * Extend to other distros

