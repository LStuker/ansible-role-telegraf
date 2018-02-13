Docker
=========

An Ansible Role that installs [Telegraf](https://docs.influxdata.com/telegraf) on RHEL/Centos 7 system.

- Add repository https://repos.influxdata.com/
- Activate stable repo
- Install telegraf agent


Requirements
------------

RHEL/Centos 7 system

Role Variables
--------------


```
telegraf_version: "1.4.1"
telegraf_package_state: present
```

# Used only for RedHat/CentOS.
```
influx_yum_repo_url: https://repos.influxdata.com/rhel/$releasever/$basearch
influx_yum_release_channel: stable
```

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: servers
      roles:
         - telegraf

License
-------

MIT

Author Information
------------------

This role was created by [Lucien Stuker](https://www.newbit.ch/)
