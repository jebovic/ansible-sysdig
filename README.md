Sysdig
======

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