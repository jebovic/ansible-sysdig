Sysdig
======

[![Build Status](https://travis-ci.org/jebovic/ansible-sysdig.svg?branch=master)](https://travis-ci.org/jebovic/ansible-sysdig) [![Ansible Galaxy](https://img.shields.io/badge/galaxy-jebovic.sysdig-blue.svg?style=flat)](https://galaxy.ansible.com/jebovic/sysdig)

Install and configure sysdig

Role Variables
--------------

```
# Sysdig install configuration
sysdig_apt_key_url: https://s3.amazonaws.com/download.draios.com/DRAIOS-GPG-KEY.public
sysdig_apt_repo: deb http://download.draios.com/stable/deb stable-$(ARCH)/
sysdig_packages:
  - sysdig
```

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - { role: jebovic.sysdig }
```

License
-------

MIT

Author Information
------------------

Jérémy Baumgarth https://github.com/jebovic