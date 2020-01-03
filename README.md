AEM Monitoring Role
=========
[![License](https://img.shields.io/badge/license-Apache-green.svg?style=flat)](https://raw.githubusercontent.com/lean-delivery/ansible-role-filebeat/master/LICENSE)
[![Build Status](https://travis-ci.org/lean-delivery/ansible-role-filebeat.svg?branch=master)](https://travis-ci.org/lean-delivery/ansible-role-filebeat)
[![Build Status](https://gitlab.com/lean-delivery/ansible-role-filebeat/badges/master/build.svg)](https://gitlab.com/lean-delivery/ansible-role-filebeat/pipelines)
[![Galaxy](https://img.shields.io/badge/galaxy-lean__delivery.filebeat-blue.svg)](https://galaxy.ansible.com/lean_delivery/filebeat)
![Ansible](https://img.shields.io/ansible/role/d/38385.svg)
![Ansible](https://img.shields.io/badge/dynamic/json.svg?label=min_ansible_version&url=https%3A%2F%2Fgalaxy.ansible.com%2Fapi%2Fv1%2Froles%2F38385%2F&query=$.min_ansible_version)


## Summary


This role:
  - installs monitoring and log management on Ubuntu, CentOS
  - copies prepared configuration file (log path, connect to elasticsearch etc.)




Role tasks
------------


- Prepare server (add elastic repo)
- [Optional] Create folder(s) for custom paths
- Install filebeat
- Copy configuration file


Requirements
------------


- Minimal Version of the ansible for installation: 2.9
- Minimal Version of the Elastic stack: 7.5
 - **Supported OS**:
   - CentOS
     - 7,8
   - Ubuntu
     - 16.04, 18.04
   - Debian
     - 8, 9


## Role Variables
--------------


You can override any variable below by setting "variable: value" in playbook.


- `variable`
Description of variable


## Advanced config parameters:


- `variable`
Description of variable


## Dependencies
------------


Nothing


Example Playbook
----------------


### Installing Filebeat 6.x version:


```yaml
- name: Install AEM monitoring
  hosts: all
  roles:
    - role: ansible-role-aem-monitoring
```


License
-------
Apache


Author Information
------------------


authors:
  - Lean Delivery Team <team@lean-delivery.com>
