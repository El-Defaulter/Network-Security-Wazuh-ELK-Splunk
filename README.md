# Network Security Monitoring with Wazuh, ELK Stack & Splunk

This project integrates **Wazuh**, **ELK Stack (Elasticsearch, Logstash, Kibana)**, and **Splunk** to provide a comprehensive solution for network security monitoring. The system is designed to collect, process, store, and analyze security event logs from endpoints, network devices, and servers to detect threats, respond to incidents, and ensure continuous security monitoring.

## Contributors:
- **Nishikanta Padhihari** - Project Lead, Developer: Designed and implemented the integration of Wazuh, ELK, and Splunk. Responsible for overall system architecture and deployment.
- **Adeeba Nizam** - Co-Developer, Security Analyst: Worked on configuring Wazuh agents, setting up ELK Stack, and implementing Splunk integration for advanced threat detection and alerting.

## Features:
- **Wazuh HIDS (Host Intrusion Detection System)** for monitoring endpoints and network devices.
- **ELK Stack** for centralized log management, processing, and real-time visualization.
- **Splunk** for advanced SIEM (Security Information and Event Management) capabilities, including anomaly detection, log correlation, and alerting.
- Real-time monitoring of system logs, network traffic, and application events to detect malicious activities.

## Project Overview
### Architecture:
- **Wazuh**: Installed as a security agent on network devices and endpoints. It monitors system logs, file integrity, rootkits, and other security events in real-time.
- **ELK Stack**:
  - **Elasticsearch** stores logs in a structured format and enables powerful search capabilities.
  - **Logstash** processes the logs and sends them to Elasticsearch for indexing.
  - **Kibana** provides a dashboard for visualizing and analyzing logs in real-time.
- **Splunk**: Used to provide advanced correlation, alerting, and reporting features for the collected logs.

### Data Flow:
1. **Wazuh Agent** installed on endpoints collects logs (e.g., syslogs, firewall logs, security alerts).
2. The logs are sent to the **Wazuh Manager**, which performs initial analysis and stores the events.
3. Logs are processed and enriched by **Logstash**, and then indexed in **Elasticsearch**.
4. **Kibana** visualizes these logs and generates security dashboards.
5. Logs are forwarded to **Splunk** for advanced correlation, machine learning-based anomaly detection, and generating incident alerts.
