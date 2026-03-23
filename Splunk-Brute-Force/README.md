# 🛡️ Project: SIEM Brute Force Detection

## Objective
The goal of this project was to deploy a SIEM solution (Splunk) to ingest local Windows Event Logs and configure alerts to detect simulated brute-force login attacks.

## Skills Learned
- Configuring data ingestion in Splunk Enterprise.
- Writing Search Processing Language (SPL) queries to filter specific Event IDs.
- Understanding Windows Security Event Logs (Specifically Event ID 4625).
- Creating data visualizations and dashboards for security monitoring.

## Tools Used
- **Splunk Enterprise** (SIEM)
- **Windows Event Viewer**

## Steps Taken
1. Installed Splunk Enterprise and configured it to monitor local Windows Security logs.
2. Intentionally generated failed login attempts to trigger Event ID 4625.
3. Queried the Splunk index using `index=* EventCode=4625`.
4. Generated a time-chart visualization to identify the exact timeframe and volume of the attack.

## Evidence
*(Drag and drop your Splunk screenshot here so it displays in the README)*
