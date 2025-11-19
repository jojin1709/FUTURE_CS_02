FUTURE_CS_02 – Cyber Security Internship (Task 2: SOC Investigation using Elastic Stack)

👤 Intern: Jojin John
🏢 Organization: Future Interns – Cyber Security Internship
📅 Task Date: 19/11/2025
🛠 Tool Used: Elastic Stack (ELK)
📂 Task: SOC Task 2 – Security Log Investigation & Alert Monitoring

📘 Task Overview

As part of my Cyber Security Internship at Future Interns, I was assigned Task 2, which focused on performing a Security Operations Center (SOC) investigation using Elastic Stack (ELK).

The goal of the task was to analyze pre-ingested log data and identify:

🔥 Malware detections

🚫 Failed login attempts

🌐 Suspicious connection attempts

📁 Unauthorized file access

🌍 Activity from public/suspicious IP addresses

This task helped build hands-on skills in SIEM, log analysis, threat hunting, and incident detection.

📂 Repository Contents
    
    FUTURE_CS_02/
    │
    ├── screenshots/                     # All investigation screenshots 
    │   ├── malware_detected.png
    │   ├── login_failed.png
    │   ├── connection_attempt.png
    │   ├── file_accessed.png
    │   ├── import_confirmation.png
    │   └── index_fields.png
    │
    ├── SOC_Task2_Incident_Report.docx   # Complete incident report
    │
    └── README.md                         # Documentation

📸 Screenshots Included (Task Requirements)

This repository contains all required screenshots for Task 2:

✔ ELK Discover view
✔ Malware Detected query results
✔ Login Failed events
✔ Connection Attempt events
✔ File Access events
✔ Index fields view
✔ Data import confirmation (50 logs ingested)

🔍 Summary of Investigation Findings

After analyzing the SOC logs in Elastic Stack:

1️⃣ Malware Detections

Detected types include:

Ransomware behavior

Rootkit signatures

Trojan detections

Worm infection attempts

Multiple user accounts were associated with infected machines.

2️⃣ Failed Login Attempts

Repeated failed login attempts for users:

david

bob

charlie

Possible brute-force attack or credential misuse.

3️⃣ Suspicious Connection Attempts

Several connection probes from suspicious IP ranges:

198.51.x.x

203.x.x.x

Suggestive of reconnaissance/scanning.

4️⃣ Unauthorized File Access

Files accessed by multiple users near the time of malware alerts.

Potential data access violation or malware payload execution.

🧩 Overall Attack Pattern

The entire activity suggests a multi-stage cyber attack:

🔍 Reconnaissance – probing via connection attempts

🔐 Credential Attack – failed login attempts

🦠 Compromise – malware detonated

📁 Post-exploitation – suspicious file access

This matches real-world intrusion patterns seen in MITRE ATT&CK framework.

🛡 Recommended Security Actions
Priority	Action
🔴 High	Isolate infected systems immediately
🔴 High	Reset credentials of affected accounts
🟠 Medium	Block suspicious public IPs
🟠 Medium	Enable multi-factor authentication (MFA)
🟡 Low	Patch & update systems
🟡 Low	Enable strict monitoring with alert rules
📚 Internship Learning Outcome

By completing this task, I gained hands-on experience in:

Using Elastic Stack as a SIEM

Investigating security incidents

Identifying Indicators of Compromise (IOCs)

Understanding attack flow and log correlation

Writing professional SOC reports
