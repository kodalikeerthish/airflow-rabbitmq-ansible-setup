# airflow-rabbitmq-ansible-setup
An end-to-end Ansible-based setup for deploying a distributed Apache Airflow cluster with RabbitMQ integration, including webserver, scheduler, workers, and Flower UI.

This repository provides a complete, production-style Ansible automation for deploying a distributed **Apache Airflow** cluster with **RabbitMQ** as the message broker.

It includes the full lifecycle: pre-install tasks, package installation, configuration, systemd setup, and service management for the following components:

### ✅ Components Deployed
- 🐇 RabbitMQ (Message broker)
- 🌐 Airflow Webserver
- ⏱️ Airflow Scheduler
- ⚙️ Airflow Workers (Multi-node ready)
- 🌸 Airflow Flower UI (Monitoring Celery queues)
- 🔒 SSL certificate support (secure deployment-ready)

### 🚀 Use Cases
- Setting up Airflow in on-prem or cloud-based VM clusters
- CI/CD pipeline integrations
- Learning, testing, or production-ready orchestration environments

### 🧰 Tech Stack
- Ansible (Role-based structure)
- Systemd (for managing services)
- RabbitMQ (backend communication)
- Apache Airflow (orchestration engine)
- Secure Linux configuration practices

### ⚠️ Important Note

This was a **working production setup** used for multiple years to run Apache Airflow across distributed nodes with RabbitMQ as the Celery broker. However, the system was later migrated to Databricks workflows for orchestration, and this Ansible role is no longer actively maintained.

As a result:
- Python or system package versions may be outdated
- RabbitMQ and Airflow configurations are based on older stable versions
- Code may require minor tweaks to align with latest Airflow 2.x or OS-level updates

Still, the overall structure, role logic, and service integration patterns remain highly relevant and reusable in real-world infrastructure deployments.
