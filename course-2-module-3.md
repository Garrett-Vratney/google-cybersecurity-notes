# Course 2 Module 3

## Topics Covered
- Logs
- SIEM Dashboards
- Common SIEM tools

---

## Log

### Definition
A record of events that occur within an organization's systems and networks

### Common Log Sources

#### Firewall Logs
- A firewall log is a record of attempted or established connections for incoming traffic from the internet. It also includes outbound requests to the internet from within the network

#### Network Log
- A network log is a record of all computers and devices that enter and leave the network. It also records connections between devices and services on the network.

#### A server log
- A server log is a record of events related to services, such as websites, emails, or file shares. It includes actions such as login, password, and username requests.

---

## Security Information and Event Management (SIEM tool)

## Definition
An application that collects and analyzes log data to monitor critical activites in an organization. Event monitoring and analysis, and automated alerts, it stores all log data in a centralized location. 
SIEM tools offer real time monitoring and tracking of security event logs. Data can be used to analyze any potential security threat, risk, or vulnerability identified.

## Metrics

### Definition
Key technical attributes, such as responsee time, availablity, and failure rate, which are used to assess the performance of a software application.

#### Real life Connection
When I interviewed the network administrator at my campus, I was able to view see the SIEM dashboard he had created which monitors daily operation metrics.

## Security Orchestration, Automation, and Response (SOAR)

### Definition
A collection of application, tools, and workflows that use automation to respond to security events, with the development of automation it is expected that common security related incidents with the use of SIEM tools is expected to become a more streamlined process

## Types of SIEM Tools

### Self-hosted
- Requires organizations to install, operate, and maintain the tool using their own physical infastructure, such as server capacity. These applications are then managed and maintained by the organizations IT department, rather tahn a third party vendor. Self-hosted SIEM tools are ideal when an organization desires physical control over confidential data.

### Cloud-hosted
- Cloud-hosted SIEM tools are maintained and managed by SIEM providers, making the tool accessible via the internet.

### Hybird
- Hybird has benefits of the cloud hosted infastructure while maintaining physical control over sensitive information and assets.

## Industry Standard SIEM Tools

### Splunk

#### Splunk Enterprise
- A self-hosted tool used to retain, analyze, and search an organizations log data to provide security information and alerts in real time.

#### Splunk Cloud
- A cloud hosted tool used to collect, search and monitor log data. Splunk cloud is helpful for organizations running on cloud or hybrid environemnts, where some of if not all of the organizations may be done in the cloud.

### Chronicle
- A cloud native tool designed to retain, anaylze and search data. Cloud native SIEM tool which retains, analyzes and searches log data to identify potential threats, risks and vulnerabilities. With the ability to collect and analyze log in filters of
- A specific asset
- A domain name
- A user
- An IP address


## Using SIEM Tools to protect organizations

### Splunk Dashboard

#### Security Posture Dashboard
- The security posture dashboard is designed for security operations centers. It displays the last 24 hours of an organization's notable security related events and trends and allows security professionals to determine if security infrastructure and policies are performing as designed.

#### Executive Summary Dashboard
- Analyzes and monitors the overall health of the organization over time. This helps security teams improve security measures which reduce risk. Security analysts may use this dashboard to provide insights to stakeholders for analyzing trends of security incidents and trends over a time frame.

#### Incident Review Dashboard
- Allows analysts to identify suspicious patterns which can occur in the event of an incident. The dashboard assists by highlighting higher risk items that need immediate review. Can be very useful as the dashboard provides a visual timeline of the events leading up to an incident.

#### Risk Analysis Dashboard
- Helps analysts identify risk for each risk object, it shows changes in risk related activity or behavior.

### Chronicle Dashboards

#### Enterprise Insights Dashboard
- Highlights recent alerts. Identifying suspicious domain names in logs known as indicators of compromise (IOCs). Each result is labeled and measured with scores of likelihood of a threat.

#### Data Ingestion and Health Dashboard
- Shows the number of event logs, log sources, and success rates of data being processed into chronicle. Helping ensure that log related issues are addressed and that the security team has access to the log data they need.

#### IOC matches Dashboard
- Indicates the top threats, risks, and vulnerabilities to the organization. Security professionals use this dashboard to observe domain names, IP addresses, and device IOCs over time in order to identify trends.

#### Main Dashboard
- The main dashboard displays a summary of information related to the organization's data ingestion, alerting, and event activity over time. This can be utilized to access a timeline of security events and identify trends.

#### Rule Detections Dashboard
Provides statistics related to incidents with the highest occurrences, severities and detections over time. Security analysts can use this dashboard to access a list of all the alerts triggered by a specific detection rule, for example alert whenever a user opens a known malicious attachment from an email. These statistics are used to then manage recurring incidents and establish mitigation tactics.

#### User sign in overview dashboard
- Provides information about user access behavior across the organization. This dashboard allows analysts to access a list of all user sign ins to identify unusual user activity.

---

## Open Source vs Proprietary

### Open Source Tools

#### Definiton
Often free to use and user friendly, open source tools come with the objective of providing users with software that is buit by the public for the public in a collaborative way. These sources are readily available and usually customizable.

### Proprietary tools
Developed and owned by a person or company, users typically pay for usage and training. Proprietary tool owners are the ones who can access and modify the tool. Proprietary software generally allows users to modify a limited number of features

## Common Open Source Security Tools

### Linux
- An open source OS, allows you to tailor the OS to your command line interface.

### Suricata
- Open source network analysis and threat detection software. Network analysis and threat detection software is used to inspect network traffic to identify suspcious behavior and generate network data logs.

---

## Key Takeaways
- SIEM tools play a major role in monitoring organizations data. Allowing for efficient management and analysis of suspicious activity on the network. New developments and the expansion of the ever inter connecting and shifting architecture SIEM technology will continue to grow as threat actors advance as well.
- Open source tools are widely used and modified in the cybersecurity profession
- SIEM tool provides dashboards that help security professionals organize and focus security efforts.
