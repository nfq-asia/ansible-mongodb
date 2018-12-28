# Ansible-mongodb

## Requirement

Edit mongodb_version in var/main.yml to install a specific version

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

## How to use

```
ansible-playbook -i hosts mongodb.yaml
```
