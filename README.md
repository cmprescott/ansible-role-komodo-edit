komodo-edit
========

Installs Komodo Edit.
TODO: Add resource configuration (http://komodoide.com/resources/install-instructions/)

Requirements
------------

Debian Linux: None
Darwin (OS X): Homebrew

Role Variables
--------------

```
# --------
# Debian based default repo
# --------
komodo_edit_debian_ppa_repo: ppa:mystic-mirage/komodo-edit
```

Dependencies
------------

Darwin: If you're lazy use geerlingguy.homebrew to install homebrew


Example Playbook
-------------------------

    - hosts: developer
      roles:
         role: komodo-edit

License
-------

BSD

Author Information
------------------

Prescott Chris
