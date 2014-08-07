Ansible deploy-logrotate
========================

This role creates configuration for logrotate.

For more information about deployment setup see this [overview](https://github.com/kunik/ansible-role-deploy-metadata/blob/master/USAGE.md)

Requirements
------------

No

Role Variables
--------------

```
deploy_logrotate:
  - name: *.log
    period: daily
    amount: 5
    truncate: yes
    sharedscripts: yes
    postrotate: 'some_command'
    prerotate: 'some_command'
    firstaction: 'some_command'
    lastaction: 'some_command'

deploy_logrotate_defaults:
  conf_dir: /etc/logrotate.d
```

Define your rotation tasks under `deploy_logrotate`

Dependencies
------------

No

License
-------

BSD
