Pocketbase
=========

Pocketbase instance as a quadlet. Designed to be used multiple times on the same server.

Requirements
------------

Podman and CentOs-based / Fedora Server

Role Variables
--------------

| option | default | description |
| --- | --- | --- |
| `pb_instance_name` | <you need to set this> | technical name for this pocketbase instance |
| `pb_instance_port` | 8081 | `please change this`. port on the server, locally, instance exposed |


Dependencies
------------

* 3n3a.podman

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

### install directly from here

add the following to your `requirements.yml`

```yaml
---
roles:
  - name: 3n3a.pocketbase
    src: git+ssh://git@github.com:22/3n3a/ansible-role-pocketbase.git
    version: master
    scm: git
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
