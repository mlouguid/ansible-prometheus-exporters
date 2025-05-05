<div align="center">

# 📌 Prometheus Exporters Deployment with Ansible

</div>

<img src="./imgs/img.png" alt="exporter promtheus" />

This repository contains an Ansible playbook to automate the installation and configuration of various Prometheus exporters on Linux servers.

## 🚀 Supported Exporters
	• Node Exporter (System metrics)
	• NGINX Exporter (NGINX metrics)
	• MySQL Exporter (MySQL/MariaDB metrics)
	• Logstash Exporter (Logstash performance metrics)
	• PHP Exporter (PHP-FPM metrics)
	• Elasticsearch Exporter (Elasticsearch cluster metrics)
	• InfluxDB Exporter (InfluxDB monitoring)
	• Redis Exporter (Redis database monitoring)

## 📂 Directory Structure
```
├── ansible
│   ├── inventories/
│   │   ├── local
│   ├── roles/
│   │   ├── node_exporter/
│   │   ├── nginx_exporter/
│   │   ├── mysql_exporter/
│   │   ├── logstash_exporter/
│   │   ├── php_exporter/
│   │   ├── elasticsearch_exporter/
│   │   ├── influxdb_exporter/
│   │   ├── redis_exporter/
│   ├── exporters_playbook.yml
│   ├── ansible.cfg
```

## 🛠 Prerequisites
	• Install Ansible (pip install ansible)
	• SSH access to target servers
	• Sudo privileges on remote machines
 
## 🎯 Installation & Deployment

Clone the repository:
```
git clone https://github.com/mlouguid/ansible-prometheus-exporters.git
cd ansible-prometheus-exporters
ansible-playbook -i inventories/local/hosts exporters_playbook.yml
```
