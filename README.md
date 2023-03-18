setup-macos
=========

A simple Ansible role to setup my macOS machine.


Requirements
------------

Homebrew and ansible needs to be installed as a minimum.
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install ansible
```


Role Variables
--------------

- **brew_pkgs**: (Optional) List of packages that are installed via homebrew. Default values come from the var file, but can be overriden at the playbook level.

- **brew_casks**: (Optional) List of GUI packages that are installed via homebrew. Default values come from the var file, but can be overrident at the playbook level.

- **omz**: (Optional, default=true) Boolean value to install the Oh My Zsh framework.

- **create_zshrc**: (Optional, default=true) Boolean value that determines if the .zshrc needs to be created from the zshrc jinja template.


Example Playbook
----------------

An example `playbook.yml` is given in this role for reference.


License
-------

BSD
