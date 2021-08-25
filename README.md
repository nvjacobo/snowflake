Role Name
=========

An Ansible Role that Snowflake proxy on GNU/Linux.

Requirements
------------

None.

Role Variables
--------------

   snowflake_user: snowflake
   snowflake_update: yes


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
          - nvjacobo.snowflake
