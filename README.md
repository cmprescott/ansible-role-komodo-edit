Ansible Role: Komodo Edit
========
[![Build Status](https://travis-ci.org/cmprescott/ansible-role-komodo-edit.svg?branch=master)](https://travis-ci.org/cmprescott/ansible-role-komodo-edit)

Installs Komodo Edit.

TODO: Add resource configuration (http://komodoide.com/resources/install-instructions/)

Requirements
------------

Debian (Linux): None

Darwin (OS X): Homebrew

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

Ubuntu (Linux): None

Debian (Linux): None

Darwin (OS X): If you don't have homebrew; use an Ansible role like geerlingguy.homebrew to install it

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
