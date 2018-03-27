Role Name
=========

<b> orahost </b>: This will configure the host specific Oracle stuff:

- Install required packages.
- Verify /etc/hosts.
- Add a user & group.
- Create directory structures.
- Generate ssh-keys and set up passwordless ssh between clusternodes in case of RAC/RAC One node.
- Handle filesystem storage (partition devices, creates vg/lv and a filesystem (ext4, xfs, btrfs) etc). If you want to create your database on a filesystem (instead of ASM) this is where you define the layout.
- Change kernel paramemeters.
- Set up pam.d/limits config.
- Configures Hugepages (as a percentage of total RAM).
- Disables transparent hugepages.
- Configure user's limits.

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
   - name: Host configuration
     hosts: all
     user: root
     roles:
        - orahost

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
