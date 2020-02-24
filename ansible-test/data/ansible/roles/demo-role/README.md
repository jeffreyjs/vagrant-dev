Role Name
=========

A demo role for changing vagrant MOTD with ansible.

Requirements
------------

None at this time

Role Variables
--------------

roles/demo-role/defalts/main.yml
# ASCII art
motd_ascii_art: 
# Default information to show under the ASCII art
motd_info: (Gathered from Ansible Facts)

Dependencies
------------

No dependencies required

Example Playbook
----------------

Simple playbook to change the MOTD of a server in vagrant with a hosts.ini file:

[vagrant]
vbox ansible_connection=local ansible_user=vagrant

    - hosts: vagrant
      roles:
         - role: demo-role

License
-------

BSD

Author Information
------------------

Jeffrey Swindel
