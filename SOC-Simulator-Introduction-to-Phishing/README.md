# SOC Simulator - Introduction to Phishing
Overview
Completed the SOC Simulator: Introduction to Phishing scenario.
This exercise focused on investigating phishing alerts,analysing suspicious emails,identifying indicators of compromise and creating SOC case reports.

## Scenario Objectives
- Monitor and analyse real time security alerts
- Identify phishing emails and suspicious links
- Investigate indicators using SIEM logs
- Classify alerts as True Positive or False Positive
- Document findings through case reports

## Skills Practised
- Phishing email analysis
- Alert triage
- Incident investigation
- SIEM investigation
- Threat indicator identification
- SOC case reporting

## Investigated Alerts
### Alert 8816 - Access to Blacklisted External URL Blocked by Firewall
Classification:True Positive
Summary:A user attempted to access a blacklisted external URL. The firewall successfully blocked the connection.

Key Indicators:
- Source IP: 10.20.2.17
- Destination IP: 67.199.248.11
- Suspicious URL: bit.ly/3sHkX3da12340
- Action: Blocked
  
### Alert 8815 - Amazon Package Phishing Email
Classification:True Positive
Summary:A phishing email impersonating Amazon was detected. The email used a fake sender domain and a shortened URL to trick the user into providing information.
Key Indicators:
- Sender: urgents@amazon.biz
- Suspicious URL: bit.ly/3sHkX3da12340
- Technique: Brand impersonation and social engineering

### Alert 8817 - Fake Microsoft Account Security Email
Classification:True Positive
Summary:A phishing email impersonating Microsoft was identified. The attacker used a looka like domain to attempt credential theft.
Key Indicators:
- Sender: no-reply@m1crosoftsupport.co
- URL: https://m1crosoftsupport.co/login
- Technique: Typosquatting and credential harvesting
Key Learnings
- Phishing attacks commonly use urgency and fear to manipulate users.
- Attackers often impersonate trusted brands such as Microsoft and Amazon.
- Email analysis requires checking sender domains, links, and user activity.
- SOC analysts must document evidence clearly before escalating alerts.
Tools Used
- SOC Simulator
- SIEM investigation
- Firewall logs
- Email analysis
