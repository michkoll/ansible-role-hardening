Role Name
=========

Ansible role for hardening server. The actual development is specific for a honeypot server.

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

No dependencies.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: hardening }

License
-------

MIT

Author Information
------------------

&copy; 2018
Written by [Michael Koll](https://github.com/michkoll)
