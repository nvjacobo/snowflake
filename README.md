Ansible Role: Snowflake proxy
=========

An Ansible Role that Snowflake proxy on GNU/Linux and FreeBSD

Requirements
------------

You need root privileges or sudo user to run this role.

Supported Operating Systems
------------
- Debian Bullseye
- Debian Buster
- Ubuntu
- ArchLinux
- Fedora  
- FreeBSD

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

Example Playbook with Variable clients
----------------

    - hosts: snowflake
       vars:
        clients: 300
      roles:
         - nvjacobo.snowflake

The above playbook has a limit of 300 concurrent clients. 
