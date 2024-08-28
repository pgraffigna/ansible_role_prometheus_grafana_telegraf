# ansible_role_prometheus_grafana_telegraf

Ansible rol para desplegar el stack TIG (telegraf + influxdb + grafana) o prometheus.

Testeado con Vagrant + qemu + ubuntu_22.04 + ansible_2.10

----

### Descripción

La idea del proyecto es automatizar vía ansible la instalación/configuración del stack TIG [telegraf](https://docs.influxdata.com/telegraf/v1/install/), [influxdb](https://docs.influxdata.com/influxdb/v2/install/), [grafana](https://grafana.com/docs/grafana/latest/setup-grafana/installation/) o en su defecto instalar [prometheus](https://prometheus.io/docs/prometheus/latest/installation/) para pruebas de laboratorio, el repo cuenta con 5 roles:

1. grafana
2. influxdb
3. mariadb
4. prometheus
5. telegraf

### Dependencias

* [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html)
* [Vagrant](https://developer.hashicorp.com/vagrant/install) (opcional)

### Uso

```
git clone https://github.com/pgraffigna/ansible_role_prometheus_grafana_telegraf.git
cd ansible_role_prometheus_grafana_telegraf
ansible-playbook main.yml
```

### Extras
* Archivo de configuración (Vagrantfile) para desplegar una VM descartable con ubuntu-22.04 con libvirt como hipervisor.

### Uso Vagrant (opcional)
```
vagrant up
vagrant ssh
```