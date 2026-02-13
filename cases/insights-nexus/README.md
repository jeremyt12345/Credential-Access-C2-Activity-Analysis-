# Insights Nexus – Credential Access & C2 Investigation

## Tools Used
- TheHive
- Wazuh
- CyberChef
- VirusTotal

## Framework Alignment
- MITRE ATT&CK
  - T1105 – Ingress Tool Transfer
  - T1555 – Credentials from Password Stores

---

## Executive Summary

Conducted structured incident investigation using TheHive and Wazuh logs; analyzed encoded PowerShell execution, extracted command-and-control (C2) infrastructure, mapped credential access behavior (T1555), and performed threat intelligence enrichment to support containment decisions.

---


Questions for Lab

1. Open the alert "[InsightNexus] Admin Login via ManageEngine Web Console." Find the foreign IP address starting with "203" in the comments. Check VirusTotal for the information related to this IP address, and add the details as a comment in this alert. In VirusTotal, what is the name of the file starting with "Mango" in the Files Referring section?

2. In VirusTotal, go to the details of the IP address starting with "198." What is the name of the city shown in the Whois Lookup?

3. If malware downloads files from a C2 (Command and Control) server into the victim network, under what MITRE technique ID does this tool transfer technique fall? Type it as your answer. The format is T1***.

4. Open TheHive and check the rule ID 92153 related to the VaultCli.dll module. What is the MITRE technique ID for this activity? The format is T1***.

5. Download the "logs-wazuh.zip" file from resources, and identify the suspicious PowerShell command in the logs. Type the suspicious IP address after decoding the command.

6. In the same file (i.e., logs-wazuh.zip), identify the user who executed the suspicious PowerShell command. The format is domain\user.
