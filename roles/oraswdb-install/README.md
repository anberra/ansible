Role Name
=========

<b>oraswdb-install</b>: This role will install the oracle database server(s). It is possible to run more than 1 database from each home. It performs both Single Instance/RAC installations.

- Creates a .profile_databasename.
- Creates directory structures.
- Transfers installfiles to server(s).
- Installs the database-server(s).

Requirements
------------

None

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

---
 - name: RDBMS Install
   hosts: all
   user: root
   roles:
      - oraswdb-install

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
