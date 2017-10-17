Role of installing Redis
=========

Redis ansible galaxy role.

Requirements
------------

None

Role Variables
--------------

* redis_version  
Install Redis version

* reids_bind_address  
using bind address

* redis_port  
using redis port

* redis_daemonize_enabled  
If you need daemonize redis, set `"yes"`

* redis_tcp_backlog  
tcp backlog

* redis_timeout  
timeout for redis

* redis_tcp_keepalive  
tcp keep alive

* redis_log_file_path  
If you need output STDOUT, set `''`

* redis_log_level  
log level

* redis_databases
redis databases

Dependencies
------------

None

Example Playbook
----------------

```yml
---
- hosts: all
  become: true
  roles:
    - { role: galaxy-redis, redis_version: 3.2.1 }
```

License
-------

BSD

Author Information
------------------

[Daisuke Maeda](https://github.com/dmae3 "Daisuke Maeda")
