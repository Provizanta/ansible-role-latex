Ansible role: Latex
=========

[![Build Status](https://travis-ci.com/Provizanta/ansible-role-latex.svg?branch=master)](https://travis-ci.com/Provizanta/ansible-role-latex)

Install LaTeX, LaTeX utilities and editors.

Requirements
------------

None

Role Variables
--------------

These defaults are set in defaults/main.yml:

    package: 'recommended'    # base|recommended|normal|extra|full

    extensions: []

    editors: []

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
        - role: latex
          vars:
            package: 'base'
            extensions:
              - texlive-extra-utils
            editors:
              - texstudio
              - texmaker

License
-------

MIT

Author Information
------------------

Tibor Csóka
