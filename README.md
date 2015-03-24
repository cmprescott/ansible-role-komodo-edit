Ansible Role: Komodo Edit
========
[![Build Status](https://travis-ci.org/cmprescott/ansible-role-komodo-edit.svg?branch=master)](https://travis-ci.org/cmprescott/ansible-role-komodo-edit)

Installs Komodo Edit 8.5

TODO: Add resource configuration (http://komodoide.com/resources/install-instructions/)

Requirements
------------

Debian: 7+ (wheezy|jessie)

Mac OS X: 10.9+ (Mavericks|Yosemite)

Ubuntu: 12.04+ (Precise|Raring|Saucy|Trusty|Utopic|Vivid)

Role Variables
--------------

```yaml
komodo_edit_pkg_install_using: One of the following (Linux_script | MacOSX_homebrew | Ubuntu_apt) 
komodo_edit_pkg_url: Url like ('http://example.com/file.tar.gz' | 'ppa:mystic-mirage/komodo-edit')
komodo_edit_dir_download: Remote directory to temporarily store installer
komodo_edit_dir_install: Remote directory to install application and lib to
```

Dependencies
------------

Mac OS X: homebrew

Debian: None

Ubuntu: None

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
