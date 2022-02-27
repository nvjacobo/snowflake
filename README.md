Ansible Role: Snowflake proxy
=========

An Ansible Role that Snowflake proxy on GNU/Linux and FreeBSD

Requirements
------------

None.

Role Variables (not for FreeBSD)
----------------

    clients: 0

Maximum concurrent clients by default is 0 = non limit

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
          - nvjacobo.snowflake
