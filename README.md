# Ansible Role: prometheus-exporters-common

This Ansible role works as a base for other roles that install Prometheus exporters.  It gives you a common user and group, as well as directories that all your exporters can use.

## Requirements

All needed packages will be installed with this role.

## Role Variables

Available variables are listed below, along with default values:
```yaml
prometheus_exporters_common_user:   prometheus
prometheus_exporters_common_group:  prometheus
prometheus_exporters_common_shell: "/sbin/nologin"

prometheus_exporters_common_root_dir: /opt/prometheus/exporters
prometheus_exporters_common_dist_dir: "{{ prometheus_exporters_common_root_dir }}/dist"
prometheus_exporters_common_log_dir:  /var/log/prometheus
prometheus_exporters_common_conf_dir: /etc/prometheus/exporters
```
## Dependencies

This role doesn't have dependencies.

## License

GPLv2
