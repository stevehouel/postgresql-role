# Posgresql Creation playbook #


## Requirements

This project must be cloned under specific project's Ansible Roles to Create Postgresql Container.

## Variables

`postgresql_path` : Postgresql Root Path for configurations and datas

`postgresql_data_path` : Postgresql Data Path (usually set to "{{ postgresql_path }}/data")

`postgresql_config_path` : Postgresql Config Path (usually set to "{{ postgresql_path }}/config")

`postgresql_logs_path` : Postgresql Logs Path (usually set to "{{ postgresql_path }}/logs")

`postgresql_port` : Listen port on Docker host to map to postgresql container

`postgresql_version` : Docker Posgresql image version

`postgresql_username` : The root username for the Postgresql first Init

`postgresql_password` : The root password


## Files

* You need to create a folder with path `conf-postgresql/postgresql.conf` to include the postgresql server Configurations, otherwise the default one will be copied.
