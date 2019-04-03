Users
=========

Create users.

Requirements
------------

Ubuntu box.

Role Variables
--------------

`users_comment` - default comment added to user account
`users` - list of users to add.

Dependencies
------------

n/a

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - role: krecik.users
       users:
        - username: tomasz.skret
          public_keys:
          - "ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAID2fd11kgzlNJNQqDMpsqLF8T95ukVTJOKZ7MUvusZN/ tomasz@tomasz-Precision-5510"
          use_sudo: yes
        - username: another.user
          use_sudo: no
```
License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
