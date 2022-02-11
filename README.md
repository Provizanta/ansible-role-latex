Ansible role: LaTeX
=========

![Build & Deploy](https://github.com/Provizanta/ansible-role-latex/workflows/molecule/badge.svg?branch=master)

Install LaTeX, LaTeX utilities and latex_editors.

Requirements
------------

None

Role Variables
--------------

These variables are defined in [defaults/main.yml](./defaults/main.yml):

    latex_package: 'recommended'    # base|recommended|normal|extra|full

    latex_extensions: []

    latex_editors: []

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
        - role: latex
          vars:
            latex_package: 'base'
            latex_extensions:
              - texlive-extra-utils
            latex_editors:
              - texstudio
              - texmaker

License
-------

MIT

Author Information
------------------

Tibor Csóka
