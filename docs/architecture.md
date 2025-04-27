# System Architecture

This project integrates **Wazuh**, **ELK (Elasticsearch, Logstash, Kibana)**, and **Splunk** for real-time monitoring, threat detection, and log analysis.

## Architecture Overview:
- **Wazuh** agents installed on endpoints and network devices collect security logs and events.
- **Logstash** ingests and processes logs from Wazuh and forwards them to **Elasticsearch**.
- **Elasticsearch** stores logs in an indexed format, enabling efficient querying.
- **Kibana** visualizes logs and security events for easy analysis.
- **Splunk** correlates logs and provides advanced analytics and alerting.

## Data Flow:
1. **Wazuh Agent** on endpoints collects logs.
2. Logs are sent to the **Wazuh Manager**.
3. The **Logstash pipeline** processes the logs and forwards them to **Elasticsearch**.
4. **Kibana** displays security events and logs for analysis.
5. **Splunk** receives logs for advanced threat detection and correlation.
