# Ansible Role: Nginx

[![Build Status](https://travis-ci.com/davidalger/ansible-role-nginx.svg?branch=master)](https://travis-ci.com/davidalger/ansible-role-nginx)

Installs nginx service from EPEL RPMs on RHEL / CentOS 7.

Currently this role installs nginx pre-configured with defaults tuned for Magento. Some of these defaults may be different if this role is used to deploy in a non-Magento environment. See `defaults/main.yml` for details.

## Requirements

None.

## Role Variables

See `defaults/main.yml` for details.

## Dependencies

* `geerlingguy.repo-epel`
* `davidalger.selinux`

## Example Playbook

    - hosts: web-servers
      roles:
        - { role: davidalger.nginx, tags: nginx }

## License

This work is licensed under the MIT license. See LICENSE file for details.

## Author Information

This role was created in 2017 by [David Alger](https://davidalger.com/) with contributions from [Matt Johnson](https://github.com/mttjohnson/).
