ansible-role-selinux
=========

SELinux configuration.

Requirements
------------

This role has only been tested on EL 6 systems.

Role Variables
--------------

__role\_selinux\_state__: Enable or disable SELinux. Values: enforcing, permissive, or disabled. Defaults to 'enforcing'.

__role\_selinux\_policy__: Set the SELinux policy to use. Defaults to 'targeted'.

__role\_selinux\_conf__: The SELinux configuration file. Defaults to '/etc/selinux/config'.

Example Playbook
----------------

Override the above variables by modifying your project's group_vars or host_vars.

```
- hosts: servers
  roles:
    - { role: bitmotive.ansible-role-selinux, tags: "selinux,common" }
```

License
-------

MIT
