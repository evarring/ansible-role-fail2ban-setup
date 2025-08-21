# fail2ban_setup

=========

Ansible role for installing and configuring fail2ban

## Role Variables

--------------

For the default jail, the role will first check if "jail.local_{{ inventory_hostname }}.j2" template exists. If it doesn't, it will use the included default jail in the role "jail.local.j2"

Other variables are more or less described in defaults/main.yml comments

## Example Playbook

--------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- name: Fail2ban setup
  hosts: all
  gather_facts: true

  roles:
    - fail2ban_setup
```
