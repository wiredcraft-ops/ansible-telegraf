## Ansible-Telegraf
> an ansible role to install, configure and manage [Telegraf](https://www.influxdata.com/time-series-platform/telegraf/)

[![xuqingfeng.telegraf](https://img.shields.io/badge/role-xuqingfeng.telegraf-blue.svg?style=flat-square)](https://galaxy.ansible.com/xuqingfeng/telegraf/)

### Installation

`ansible-galaxy install xuqingfeng.telegraf -p roles`

### Role Variables

```yaml
#vars/main.yml
telegraf_version: 1.2.1 #telegraf version number; get from https://www.influxdata.com/downloads/

#default/main.yml
#...
```

**Full config [here](https://github.com/influxdata/telegraf/blob/master/etc/telegraf.conf)**

### Example Playbook

```yaml
- hosts: server
  roles:
    - role: xuqingfeng.telegraf
      telegraf_custom_config_files: ["/etc/telegraf/telegraf.d/*.conf"]
```

### Docker

[https://github.com/influxdata/influxdata-docker/tree/master/telegraf](https://github.com/influxdata/influxdata-docker/tree/master/telegraf)



