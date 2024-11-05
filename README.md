# SIEM Project: Log Analytics and Geographic Data Enrichment

## Overview

This project demonstrates the integration of Microsoft Azure Sentinel with a log repository, leveraging PowerShell scripts to extract IP address data from Windows logs and enrich it with geographic details. The enriched data is then stored in a custom log format, enabling enhanced security monitoring and analysis.

## Key Features

- **Virtual Machine (VM)**: A virtual machine exposed for capturing logs and performing analysis.
- **Log Repository**: Set up using Azure Log Analytics Workspace to centralize and store log data.
- **Azure Sentinel**: Deployed to visualize and analyze security events, including attack origin data using a map.
- **Geographic Enrichment**: PowerShell script extracts IP addresses from Windows logs and sends them to a third-party API, which returns geographic data (latitude, longitude, state, province, etc.).
- **Custom Log Creation**: Geographic information is added to the logs, enabling more detailed event analysis.

## Technologies Used

- **Microsoft Azure**: Utilized for deploying VM, Log Analytics Workspace, and Sentinel for log management and security monitoring.
- **PowerShell**: Used for scripting the extraction of IP addresses from Windows logs and interfacing with the third-party API to fetch geographic data.
- **Third-party API**: For IP-to-geolocation lookups, enriching the logs with geographic information.

## Usage
Once the environment is set up, Sentinel will automatically pull logs from the Log Analytics Workspace and visualize attack data on the map.
The custom log file containing enriched geographic data will be updated as new logs are processed.
Security analysts can use the Sentinel dashboard to monitor and investigate security events based on both IP addresses and their geographic origins.


## Conclusion
This SIEM solution helps enhance security monitoring by not only providing detailed logs from Azure Sentinel but also enriching those logs with valuable geographic context. By integrating Windows logs with a geolocation API, security teams can better understand the origins of attacks and make more informed decisions.

<p align="center">
Log Analytics Extraction:  <br/>
<img src="https://imgur.com/pm8s3C2.png" height="90%" width="90%" alt="SIEM"/>
<br />
<br />
Log Analytics Extraction Part 2: <br/>
<img src="https://imgur.com/kERIE0j.png" height="90%" width="90%" alt="SIEM"/>
<br />
<br />
Virtual Machine Access and Powershell Script with Failed Login Attempt:  <br/>
<img src="https://imgur.com/btg8msa.png" height="90%" width="90%" alt="SIEM"/>
<br />
<br />
World Map Real-Time Attacks with Script Running:  <br/>
<img src="https://imgur.com/x1Ha5H4.png" height="90%" width="90%" alt="SIEM"/>
<br />
<br />
World Map 1000+ Attack Attempts:  <br/>
<img src="https://imgur.com/otiAbrU.png" height="90%" width="90%" alt="SIEM"/>
<br />
<br />
World Map Extraction Script:  <br/>
<img src="https://imgur.com/2vvAgm7.png" height="90%" width="90%" alt="SIEM"/>
<br />
<br />
