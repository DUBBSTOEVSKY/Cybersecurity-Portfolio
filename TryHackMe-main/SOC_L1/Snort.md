# TryHackMe: Snort Room Summary

## Introduction

This TryHackMe Snort room was a challenging yet invaluable learning experience. IT provided me with hands-on knowledge of Snort, a powerful open-source network intrusion detection system (NIDS) and intrusion prevention system (IPS). Despite the hurdles, I persevered and learned how to install, configure, and use Snort to detect and respond to network threats.

## Key Topics Covered in the Lab

1. **Introduction to Snort**
   - Gained an understanding of Snort, it's parameters, and its capabilities as a NIDS/IPS.
   - Differentiated between detection and prevention systems.

2. **Installing Snort**
   - Followed a step-by-step guide to install Snort on a Linux system.
   - Managed dependencies and prerequisites for Snort installation.

3. **Snort Configuration**
   - Configured the `snort.conf` file with basic settings.
   - Set up network variables and paths.
   - Configured output modules for logging and alerting.

4. **Snort Rules**
   - Learned the structure and syntax of Snort rules.
   - Explored different types of rules: header and options.
   - Wrote custom rules to detect specific patterns and threats.

5. **Running Snort**
   - Utilized command-line options to run Snort in different modes.
   - Tested Snort configurations and rules.
   - Ran Snort in IDS mode to monitor network traffic.

6. **Analyzing Snort Alerts**
   - Interpreted Snort alert formats and logs.
   - Used tools like Barnyard2 to manage and analyze Snort alerts.
   - Integrated Snort with other tools for enhanced analysis.

## Detailed Learnings

### Introduction to Snort

Snort has become an essential tool in my cybersecurity toolkit. It provides real-time traffic analysis and packet logging, making it indispensable for network security monitoring. This enables aspiring security know-it-alls like myself to detect and respond to potential threats effectively.

### Snort Rules

Writing Snort rules was one of the most fascinating and challenging parts of this room. I learned that Snort rules are composed of two main parts: the rule header and the rule options. 

```plaintext
alert icmp any any -> any any (msg:"ICMP Echo Request"; itype:8; sid:1000001; rev:1;)
```
### Running Snort

Running Snort in different modes was essential for understanding its operation. I used commands to run Snort in IDS mode and packet logger mode. 

### Analyzing Snort Alerts

Analyzing Snort alerts involved understanding the alert format and using tools like Barnyard2 to process and manage alerts. Integrating Snort with tools like SIEM systems provided comprehensive threat analysis and response capabilities.

## Conclusion

Completing this TryHackMe Snort room was a challenging yet immensely rewarding journey. Despite the difficulties sifting through packet logs, I was determined and fueled by coffee. Eventually, my perseverance paid off. Cheers to honing skills in network intrusion detection and prevention. The hands-on experience of installing, configuring, and running Snort, along with writing custom rules and analyzing alerts was the type of journey I needed to get my hands dirty.