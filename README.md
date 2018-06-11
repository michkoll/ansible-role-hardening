Role Name
=========

Configurable ansible role für hardening server

Requirements
------------

If you are deploying to an aws instance, make sure, that the default ssh port and the new ssh port are allowed as inbound rules.

Role Variables
--------------

A list of available role variables with short explanation an default values (`default/main.yml`)

```
# Changes the ssh port.
hardening_ssh: True
```
Activate or deactivate hardening options

```
hardening_ssh_port: 49222
```
Change ssh port to the specified port. The port (default or configured) has to be set as `ansible_port` in the inventory variables.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
