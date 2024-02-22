## Overview
```
Analyze the situation using the National Institute of Standards and
Technology's Cybersecurity Framework (NIST CSF).

The CSF is a voluntary framework that consists of standards,
guidelines, and best practices to manage cybersecurity risk.

Creating a quality cybersecurity incident report and applying the
CSF can demonstrate a proactive approach to security, improving
communication and transparency with stakeholders, and improve
security practices within an organization. 
```

## Task
```
Create an incident report using NIST CSF
```

## Description
```
I am a cybersecurity analyst working for a multimedia company that
offers web design services, graphic design, and social media
marketing solutions to small businesses. Your organization
recently experienced a DDoS attack, which compromised the
internal network for two hours until it was resolved.
```

## Incident Report Analysis
### Summary
```
The company experienced a security event that caused all network services to stop responding.
The security team discovered that a DDoS attack that exploited an unconfigured firewall resulted
in a two-hour outage. Because of this, the team responded by blocking the attack, stopping
all non-critical network services, and restoring critical network services.
In addition, we wrote a report including five core functions following NIST CSF.
```
### identify
```
The company suffered an ICMP flood attack that affected its entire internal network.
Additionally, all critical network resources had to be protected and restored.
```
### Protect
```
We implemented new firewall rules to rate-limit ICMP packets, and an IDS/IPS system
to filter some ICMP traffic based on suspicious characteristics. We can also protect
against future attacks by establishing policies and training to ensure a safe environment.
```
### Detect
```
We configured source IP address checking on the firewall to check for spoofed IP
addresses in incoming ICMP packets, and implemented network monitoring software to filter out
unusual traffic.
```
### Respond
```
Isolate affected systems to prepare for future security events.
Additionally, we analyze and attempt to restore critical systems and services that have been disrupted.
Documents and reports incidents to senior management and legal authorities.
```
### Recover
```
We  restore all affected systems to normal operation.
Removes all malware and recovers data through backup.
```
### Reflections/Notes
