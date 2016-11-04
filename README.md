## Ansible-Telegraf
> an ansible role to install, configure and manage [Telegraf](https://www.influxdata.com/time-series-platform/telegraf/)

[![xuqingfeng.telegraf](https://img.shields.io/badge/role-xuqingfeng.telegraf-blue.svg?style=flat-square)](https://galaxy.ansible.com/xuqingfeng/telegraf/)

### Installation

`ansible-galaxy install xuqingfeng.telegraf -p roles`

### Role Variables

```yaml
#vars/main.yml
telegraf_version: 1.0.1 #telegraf version number

#default/main.yml
#...
```
### Dependencies

### Example Playbook

```yaml
- hosts: server
  roles:
    - xuqingfeng.telegraf
```





