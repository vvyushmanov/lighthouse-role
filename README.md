Lighthouse-role
=========

A role to install Lighthouse 

#### Lighthouse:
- Install `git`
- Get Lighthouse repository (pre-defined in variables)
- Set up nginx to run Lighthouse (port 8123)
- Make sure SELinux access to the files is granted

Requirements
------------

A web server (e.g. Nginx) required

Role Variables
--------------

| Variable name | Description |
| ------------- | ----------- |
| lh_repo | Location of the Lighthouse repository |
| lh_location | Installation path for Lighthouse |


Example Playbook
----------------

```yaml
- name: Install Lighthouse
  hosts: lighthouse
  tags: lighthouse, full
  roles:
    - lighthouse-role
```

License
-------

MIT

