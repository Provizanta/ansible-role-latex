Ansible role: LaTeX
=========

![Build & Deploy](https://github.com/Provizanta/ansible-role-latex/workflows/molecule/badge.svg?branch=master)

Install LaTeX and LaTeX extensions.

Requirements
------------

None

Role Variables
--------------

These variables are defined in [defaults/main.yml](./defaults/main.yml):

    latex_package: 'recommended'    # base|recommended|normal|extra|full

    latex_extensions: []

Dependencies
------------

None

Example Playbook
----------------

    - name: Converge
      hosts: all
      roles:
        - role: latex
          vars:
            latex_package: 'base'
            latex_extensions:
              - texlive-extra-utils

License
-------

MIT

Author Information
------------------

Tibor Csóka
