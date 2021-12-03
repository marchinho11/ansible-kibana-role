Kibana role
=========

Роль для установки kibana на хостах с ОС: Debian, Ubuntu, CentOS, RHEL.

Requirements
------------

Поддерживаются только ОС семейств debian и EL.

Role Variables
--------------

| Variable name | Default | Description |
|-----------------------|----------|-------------------------|
| kibana_version | "7.14.0" | Параметр, который определяет какой версии kibana будет установлен |
| elastic_address | "0.0.0.0:9200" | Параметр, который определяет адрес elastic |

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: kibana_role }
