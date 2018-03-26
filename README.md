borg-backup
===========

Borg Backup client to automatically send encrypted backups to a remote repo.

Requirements
------------

Host must be able to reach a borg-repo (can be remote or local).

Role Variables
--------------

- `borg_repo`

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      pre_tasks:
        - import_vars: private_keys_vault
        - import_vars: borg_auth_users
      roles:
         - { role: thinkmassive.borg-backup }

License
-------

Apache

Author Information
------------------

Alexander Miller alex@thinkmassive.org
