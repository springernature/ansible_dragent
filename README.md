dragent
======

Install [dragent](http://www.sysdig.org/)

Requirements
------------

This role requires Ansible 2.0+
tested on debian based OS, should work on redhat systems aswell

Role Variables
--------------

- `api_key`: (mandatory) to setup the proper configuration of dragent and talk with your sysdigcloud account 
- `dragent_tags`: (optional), can be used to sysdigcloud's tagging feature to create a custom structure of your environment

Dependencies
------------

None

Example Playbook
----------------

Install dragent
```yaml
- hosts: all
  vars:
  	- dragent_tags:
  		- name: role
  		  value: testinstance
  		- name: location
  		  value: openstack_cluster
  		- name: az
  		  value: rotterdam
    - dragent_api_key: put-your-customer-id-here
  roles:
  - ansible_dragent

```

License
-------

CC-BY 2.0

Author Information
------------------

Lukas Wingerberg
