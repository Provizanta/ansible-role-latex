Ansible role: Latex
=========

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
              - extra-utils
            editors:
              - texstudio
              - texmaker

License
-------

MIT

Author Information
------------------

Tibor Csóka
