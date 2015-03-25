Ansible Role: Komodo Edit
========
[![Build Status](https://travis-ci.org/cmprescott/ansible-role-komodo-edit.svg?branch=master)](https://travis-ci.org/cmprescott/ansible-role-komodo-edit)

Installs Komodo Edit 8.5

TODO: Add resource configuration (http://komodoide.com/resources/install-instructions/)

Requirements
------------

- [Darwin](http://docs.activestate.com/komodo/8.5/install.html#System_Req_OSX "Mac OS X Requirements")
  - **Mac OS X:** 10.9+ (Mavericks|Yosemite)
- [Linux](http://docs.activestate.com/komodo/8.5/install.html#System_Req_Lin "Linux Requirements")
  - **CentOS:** 6.0+
  - **Debian:** 7+ (wheezy|jessie)
  - **Fedora Core:** 15+
  - **OpenSUSE:** 12.1+
  - **SuSE Linux Enterprise Desktop/Server:** 11.3+ 
  - **Ubuntu:** 12.04+ (Precise|Raring|Saucy|Trusty|Utopic|Vivid)

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

- **Darwin (Mac OS X)**: homebrew
- **Linux**: None

TODO: Bake homebrew dependency into meta file

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
