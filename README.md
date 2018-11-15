Latex
=========

Install LaTeX, LaTeX utilities and editors.

Requirements
------------

None

Role Variables
--------------

    package: <type of package, one of [base, recommended, normal, extra, full], defaults to 'recommended'>    
    extensions: <list of latex extensions without the 'latex-' prefix>
    editors: <list of latex editors to be installed>

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

Tibor Csoka
