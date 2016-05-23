Role Name
=========

Installs and configures the Apache mod_evasive module

Created to support Debian
Will have wider support soon.

Requirements
------------

Assumes that Apache is installed and running

Role Variables
--------------

see default file for variables

Dependencies
------------

Apache

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: weservers
      roles:
         - { role: ansible-role-modevasive, tage: mod_evasive }


Notes:
----------------

DOSSystemCommand    "sudo /sbin/iptables -A INPUT -s %s -j DROP && sudo /sbin/iptables -D INPUT -s %s -j DROP | at now + 2 hours"

see https://bloke.org/linux/prevent-dosddos-attacks-with-apache-and-mod_evasive/

DOSSystemCommand "/bin/echo hi >> /tmp/out.txt"

https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=603392

License
-------

BSD

Author Information
------------------

George Boobyer (Blue-Bag)
