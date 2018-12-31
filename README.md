# Ansible-mongodb

## Requirement

Edit mongodb_version in defaults/main.yml or in the mongdb.yml playbook to install a specific version

## Role Variables

- mongodb_source_key
- mongodb_source_url
- mongodb_verion

## mongdb.yaml

- hosts: all
  gather_facts: false
  become: true
  roles:
  - ansible-mongodb
  vars:
    mongodb_version: "4.0"

## How to use

```
ansible-playbook -i hosts mongodb.yaml
```
