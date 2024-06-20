# Junior Security Analyst Intro
================================

## Introduction

This document provides an overview of my journey through the Junior Security Analyst intro class on TryHackMe. It covers fundamental concepts such as the role of a security analyst, the structure and function of a Security Operations Center (SOC), and what a typical day looks like for a security analyst.

## Topics Covered

### 1. What is a Security Analyst?

A security analyst is responsible for protecting an organization’s information systems by identifying and responding to potential threats. Key responsibilities include:

- **Monitoring**: Keeping an eye on security alerts and logs to detect suspicious activities.
- **Analysis**: Investigating potential security incidents to determine their nature and impact.
- **Response**: Implementing measures to contain and remediate security threats.
- **Reporting**: Documenting incidents and providing detailed reports for further review and compliance.

### 2. What is a Security Operations Center (SOC)?

A Security Operations Center (SOC) is a centralized unit that deals with security issues on an organizational and technical level. It serves as the hub for monitoring, detecting, responding to, and managing cybersecurity incidents. Key components of a SOC include:

- **People**: Trained security analysts and incident responders.
- **Processes**: Standardized procedures for incident detection, analysis, and response.
- **Technology**: Tools and platforms for monitoring, analysis, and reporting.

### 3. A Day in the Life of a Security Analyst

A typical day for a security analyst in a SOC involves various tasks and activities aimed at maintaining and improving an organization’s security posture. Some of the daily tasks include:

- **Log Analysis**: Reviewing logs from various sources to identify anomalies or potential security incidents.
- **Alert Triage**: Prioritizing alerts based on their severity and potential impact.
- **Incident Response**: Investigating and responding to security incidents, including containment, eradication, and recovery.
- **Communication**: Collaborating with other teams and stakeholders to provide updates and share information about ongoing incidents.
- **Continuous Improvement**: Participating in training and staying updated with the latest security trends and best practices.

### 4. Introduction to SIEM Ticket Pipeline

During the course, I was introduced to the SIEM (Security Information and Event Management) ticket pipeline. This system is crucial for tracking and managing security incidents from detection to resolution. One practical scenario I encountered involved the following steps:

1. **Detection of a Malicious IP**: A suspicious IP address (221.181.185.159) was detected after making a successful SSH connection on its second attempt.
2. **Escalation**: The incident required contacting the appropriate person. In this case, it was the SOC Team Lead, Will Griffin.
3. **Response Instructions**: Will Griffin provided instructions to add the malicious IP address to the block list.
4. **Action Taken**: I added the IP address to the firewall's block list.
5. **Resolution**: Upon blocking the IP, I received a message stating "THM{UNTIL-WE-MEET-AGAIN}".

This exercise highlighted the importance of clear communication and swift action in handling security incidents.

### 5. Pyramid of Pain

The Pyramid of Pain is a model that illustrates the difficulty of disrupting an adversary's operations based on the type of indicators used. The higher up the pyramid, the more pain it causes to the adversary when those indicators are detected and blocked. The levels of the pyramid are:

1. **Hash Values**: Unique identifiers for specific files.
2. **IP Addresses**: Addresses used by adversaries to communicate.
3. **Domain Names**: Domains registered by adversaries.
4. **Network/Host Artifacts**: Specific patterns or behaviors on the network or host.
5. **Tools**: Software used by adversaries.
6. **Tactics, Techniques, and Procedures (TTPs)**: Adversary behaviors and methods.

### 6. Hash Values and Malware Analysis

Hash values are used to uniquely identify specific malware samples. They provide insights into the malware's properties and can be used to detect and block malicious files. The most common hashing algorithms include:

- **MD5**: Produces a 128-bit hash value.
- **SHA1**: Produces a 160-bit hash value.
- **SHA2**: Produces hash values of varying lengths (e.g., 256-bit, 512-bit).

### 7. Tools for Malware Analysis

To analyze malware and verify its hash values, I learned about the following tools:

- **VirusTotal**: An online service that aggregates multiple antivirus engines and scan results to analyze files and URLs for malware.
- **OPSWAT**: A platform that provides threat intelligence and tools for malware analysis.

### 8. Cyber Kill Chain

The Cyber Kill Chain is a model developed by Lockheed Martin that outlines the steps taken by adversaries during a cyberattack. Understanding this model helps in detecting and responding to threats at various stages. The stages of the Cyber Kill Chain include:

1. **Reconnaissance**: Gathering information about the target.
2. **Weaponization**: Creating malicious payloads.
3. **Delivery**: Sending the payload to the target.
4. **Exploitation**: Exploiting vulnerabilities to execute the payload.
5. **Installation**: Installing malware on the target system.
6. **Command and Control (C2)**: Establishing a communication channel with the compromised system.
7. **Actions on Objectives**: Performing the intended malicious activities.

#### Tools for Reconnaissance

During the course, I learned about various tools used for reconnaissance in the Cyber Kill Chain:

- **TheHarvester**: A tool used to gather emails, subdomains, hosts, employee names, open ports, and banners from different public sources.
- **Hunter.io**: A tool for finding and verifying professional email addresses.
- **OSINT (Open Source Intelligence)**: Techniques and tools used to gather publicly available information for intelligence purposes.

## Conclusion

The Junior Security Analyst intro class provides a solid foundation for understanding the roles and responsibilities of a security analyst, the structure and function of a SOC, and the day-to-day activities involved in maintaining cybersecurity. As I progress through this course, I will continue to document my learnings and insights.

## Future Topics

- **Incident Response Strategies**: Detailed strategies for effective incident response.
- **Threat Intelligence**: Gathering and utilizing threat intelligence to improve security defenses.
- **Security Tools**: Overview of essential tools used by security analysts in a SOC.


