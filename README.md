Ansible Role: Snowflake proxy
=========

An Ansible Role that installs and configures Snowflake proxy on GNU/Linux and FreeBSD

Background
------------
Snowflake proxies are one of the systems that the Tor network has in place to address censorship. This type of bridge, currently under development, adds to the alternatives and anti-censorship efforts of Pluggable Transports (PTs) such as obfs4 and meek-azure. Bridges designed as access options for people where the Tor network is blocked. More info [https://snowflake.torproject.org/](https://snowflake.torproject.org/)

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
