# Setup Guide

This guide will walk you through setting up **Wazuh**, **ELK Stack**, and **Splunk** for network security monitoring.

### Prerequisites:
- **Ubuntu 20.04+** or any Linux-based server
- **Wazuh** and **ELK Stack** already installed on your system.
- **Splunk** installed on the same or separate server.

### 1. Install Wazuh Manager:
- Download and install the Wazuh manager from [Wazuh Official](https://wazuh.com/).
- Configure the manager to collect logs from endpoints (see `wazuh-manager.conf` in `config/`).

### 2. Install Wazuh Agent:
- Install the Wazuh agent on your endpoints and configure it to send logs to the Wazuh manager.
- Update the `wazuh-agent.conf` configuration file (see `config/`).

### 3. Install Logstash:
- Install Logstash for log ingestion:
  ```bash
  sudo apt-get install logstash
