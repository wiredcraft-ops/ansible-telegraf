## Ansible-Telegraf
> an ansible role to install, configure and manage [Telegraf](https://www.influxdata.com/time-series-platform/telegraf/)

### Installation

```
# requirements.yml
- src: https://github.com/wiredcraft-ops/ansible-telegraf.git
  name: wcl-telegraf
  version: master
```

```bash
ansible-galaxy install -r requirements.yml -p roles
```

### Role Variables

```yaml
# default/main.yml
telegraf_version: 1.2.1 # telegraf version number; get from https://www.influxdata.com/downloads/
# ...
```

**Full config [here](https://github.com/influxdata/telegraf/blob/master/etc/telegraf.conf)**

### Example Playbook

```yaml
- hosts: server
  roles:
    - role: wcl-telegraf
      telegraf_custom_config_files: ["/CUSTOM_TELEGRAF_CONFIG_FILES/*.conf"]
```

### Docker

[https://github.com/influxdata/influxdata-docker/tree/master/telegraf](https://github.com/influxdata/influxdata-docker/tree/master/telegraf)



