# **Ansible-NGINX**

Ansible-NGINX is an Ansible role for installing and configuring NGINX for Debian and Ubuntu systems using NGINX official apt repository. At the moment, the role only installs NGINX and makes changes to its configuration structure. This role cannot be used for configuring NGINX server blocks.

## **Requirements**
At the moment this role is being written for Debian based distributions e.g. Debian/Ubuntu. It may evolve to include other major distributions.

## **Role Variables**

See `defaults/main.yml` and `vars/main.yml` file for a list of variables used to create `/etc/nginx/nginx.conf` file.

## **Dependencies**

This role doesn't depends on any other role for execution.

## **Example Playbook**

Facts gathering must be enabled.

An example of running the role is as follows:
```yaml
- hosts: servers
  gather_facts: True
  roles:
    - Ansible-NGINX
```
## **License**

This playbook is licensed under MIT License (See the LICENSE file).

## **Author**

[Saad Ali](https://github.com/nixknight)