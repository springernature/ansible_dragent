dragent
======

Install [dragent](http://www.sysdig.org/)

Requirements
------------

This role requires Ansible 2.0+

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

Install dragent
```yaml
- hosts: all
  vars:
    api_key: put-your-customer-id-here
  roles:
  - ansible_dragent

```

License
-------

CC-BY-NC

Author Information
------------------

Lukas Wingerberg
