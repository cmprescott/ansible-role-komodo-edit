Ansible Role: Komodo Edit
========
[![Build Status](https://travis-ci.org/cmprescott/ansible-role-komodo-edit.svg?branch=master)](https://travis-ci.org/cmprescott/ansible-role-komodo-edit)

Installs Komodo Edit 8.5.

TODO: Add resource configuration (http://komodoide.com/resources/install-instructions/)

Requirements
------------

Darwin (OS X): 10.9+ (Mavericks|Yosemite)

Debian (Linux): 7+ (wheezy|jessie)

Ubuntu (Linux): 12.04+ (Precise|Raring|Saucy|Trusty|Utopic|Vivid)

Role Variables
--------------

```yaml
# --------
# Debian defaults
# --------
komodo_edit_debian_url: http://downloads.activestate.com/Komodo/releases/8.5.4/Komodo-Edit-8.5.4-14424-linux-x86_64.tar.gz
komodo_edit_debian_dir_download: /tmp
komodo_edit_debian_dir_install: /usr/local/komodo-edit

# --------
# Ubuntu default repo
# --------
komodo_edit_ubuntu_ppa_repo: ppa:mystic-mirage/komodo-edit
```

Dependencies
------------

Darwin (OS X): homebrew

Debian (Linux): None

Ubuntu (Linux): None

Example Playbook
-------------------------

```yaml
- hosts: developer
  roles:
    - { role: ansible-role-komodo-edit, sudo: Yes }
```

License
-------

BSD

Author Information
------------------

Prescott Chris
