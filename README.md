local_openssh_client_permission (1.0.2-dev)
===========================================

Fix permissions of local openssh client config files, see the manual of openssh: http://man.openbsd.org/ssh

This role can skipped if ssh client config is not present or connection is not `smart` or `ssh`,
and should be called every time when the local config is created, changing modes or we change the `ansible_connection`.

Requirements
------------

Python modules:
- andible>=2.0
- jinja2>=2.6

Role Variables
--------------

N/A

Dependencies
------------

- `gzm55.require_implicity_localhost`
- `gzm55.require_disabe_become`
- `gzm55.local_id_plugin`

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: gzm55.local_openssh_client_permission

License
-------

BSD
