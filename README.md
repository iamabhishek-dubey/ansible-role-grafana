# Ansible Role: Grafana
An ansible role for installing and configuring Grafana Server for awesome visualization.

**[Grafana Server](https://grafana.com/grafana/download)**

## Requirments
No requirments for this role :-)

## Role Variables
### Mandatory Variables
**There is no mandatory variables**

### Optional Variables
Here is the list of optional variables:-

|**Variables**|**Default Value**|**Description**|
|-------------|-----------------|---------------|
|**datasource_name**|prometheus|Name of the datasource for grafana|
|**datasource_url**|http://prometheus:9090| Url of datasource|
|**grafana_version**|5.2.2|Version of grafana which needs to install|

## Dependencies
None :-)

## Example Playbook
Here is an example playbook:-
```yml
---
- hosts: exporter
  user: ubuntu
  become: yes
  roles:
    - iamabhishek-dubey.ansible-role-grafana
```

## Usage
This is an example of how to run this role

```shell
ansible-playbook -i hosts site.yml
```

## Author
**[Abhishek Dubey](https://github.com/iamabhishek-dubey)**
