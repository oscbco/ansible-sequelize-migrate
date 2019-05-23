Role Name
=========

Execute sequelize migrations

Requirements
------------

Role Variables
--------------

userdba: OS User responsible for executing the migrations, must have the proper permissions in the target database
appdir: Your application directory, in there sequelize expects to find directories created by sequelize-cli init.

Dependencies
------------

Example Playbook
----------------

    - hosts: servers
      roles:
        - {
            role: oscbco.sequelize_migrate,
            userdba: "{{ global_userdba }}",
            appdir: "{{ global_appdir }}"
          }

License
-------

MIT

Author Information
------------------

oscbco.me
