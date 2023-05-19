# ansible_role_prometheus_grafana_telegraf

Ansible Playbook para crear un servicio de monitoreo usando prometheus + grafana + telegraf 

Testeado con Vagrant + qemu + ubuntu_20.04 + ansible_2.10

----

roles:
- telegraf
- prometheus
- grafana

----

archivos:
- prometheus.yml.j2
- telegraf.conf.j2