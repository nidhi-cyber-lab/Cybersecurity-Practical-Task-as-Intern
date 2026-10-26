# Task 16: HTTP and HTTPS Analysis (16 Oct 2026)

## Internship Details
- **Organization:** Vedatechnology
- **Track:** Cyber Security
- **Task Number:** 16
- **Task Name:** HTTP and HTTPS

## Objective
To compare HTTP and HTTPS and understand the security benefits of TLS using Google Chrome Developer Tools.

## Tools Used
- Google Chrome
- Chrome Developer Tools
- Network tab
- Internet connection

## Practical Work Performed
1. Opened the NeverSSL website to inspect HTTP communication.
2. Opened Chrome Developer Tools using the F12 key.
3. Selected the Network tab and reloaded the webpage.
4. Inspected the request headers, request method, and status code.
5. Observed the HTTP request using the GET method with a status code of 200 OK.
6. Compared HTTP with HTTPS to understand the role of TLS in secure web communication.

## HTTP vs HTTPS

| Feature | HTTP | HTTPS |
|---|---|---|
| Full form | Hypertext Transfer Protocol | Hypertext Transfer Protocol Secure |
| Encryption | No TLS encryption | Uses TLS encryption |
| Default port | 80 | 443 |
| Data integrity | No TLS-based integrity protection | TLS protects data integrity |
| Security | No TLS protection | Provides TLS-protected communication |

## Security Benefits of TLS
- **Encryption:** Protects data from being easily read during transmission.
- **Authentication:** Helps verify the server's identity using its digital certificate.
- **Data Integrity:** Helps detect unauthorized changes to transmitted data.

## Result
The HTTP request was inspected using Chrome Developer Tools. The request method, status code, and URL were observed. The comparison helped explain how HTTPS uses TLS to improve communication security.

## Conclusion
HTTPS is preferred over HTTP for secure web communication because TLS provides encryption, authentication, and data integrity.

## Evidence
Practical screenshots are in report can be added to this repository to document the work performed.

# Task 17: Firewall Fundamentals (17 Oct 2026)

## Overview

This project was completed as part of my Cybersecurity Internship task with Veda Technology.

The task focuses on understanding firewall fundamentals and creating a simple conceptual firewall policy to demonstrate how network traffic can be allowed or denied.

## Objective

- Understand the purpose of a firewall.
- Learn the basics of network traffic filtering.
- Identify allowed and denied traffic categories.
- Create a sample firewall policy.
- Understand packet-filtering and stateful firewalls.

## Topics Covered

1. Introduction to firewalls
2. How firewalls work
3. Types of firewalls
4. Allowed and denied network traffic
5. Sample firewall rules
6. Firewall security best practices
7. Common firewall interview questions

## Sample Policy

| Traffic | Action |
|---|---|
| Required outgoing HTTPS traffic | Allow |
| DNS requests to approved servers | Allow |
| Authorized SSH administration | Allow with restrictions |
| Unsolicited incoming connections | Deny |
| Traffic to known malicious destinations | Deny and log |
| Other unapproved traffic | Deny by default |

## Tools Used

- Google Docs for preparing the report and documenting the policy.
- Markdown for documenting the project.

## Key Learning

This task improved my understanding of network security, firewall rules, traffic filtering, and basic security policy documentation.

## Conclusion

Firewalls help protect networks by controlling traffic according to predefined rules. A clear firewall policy supports secure communication and reduces unnecessary network exposure.

## Disclaimer

This project is an educational, conceptual exercise. It does not represent a tested or deployed firewall configuration. Actual rules should be reviewed and tested before real-world use.

# Task 18: VPN Fundamentals (18 Oct 2026)

## Objective
To understand VPN architecture and explain how Virtual Private Networks protect network traffic over untrusted networks.

## Introduction
A Virtual Private Network (VPN) creates an encrypted connection between a user's device and a VPN server or private network. This connection is commonly called an encrypted tunnel. It helps protect data while using untrusted networks, such as public Wi-Fi.

## How a VPN Works
1. The user connects to a VPN using a VPN client.
2. The VPN system authenticates the user or device.
3. A secure connection is established between the device and the VPN server.
4. Network traffic covered by the VPN is encrypted.
5. The encrypted traffic travels through the internet to the VPN server.
6. The server forwards traffic to its destination according to the VPN configuration.

## Types of VPN
- Remote-Access VPN
- Site-to-Site VPN
- Client-Based VPN
- SSL/TLS VPN

## Benefits of VPN
- Protects data in transit through encryption.
- Helps improve security when using public Wi-Fi.
- Supports secure remote access to organizational resources.
- Connects separate office networks securely.
- Helps protect traffic between VPN endpoints.

## Limitations
A VPN does not guarantee complete anonymity. Websites can still track users through cookies, account logins, and browser fingerprinting. VPNs also do not automatically protect against malware, phishing, or every cyberattack.

## Security Best Practices
- Use a trusted VPN provider or organization-approved VPN.
- Enable multi-factor authentication where available.
- Keep the VPN application and operating system updated.
- Use HTTPS websites.
- Avoid suspicious links and downloads.
- Review the VPN provider's privacy policy.

## Tools Used
- Web Browser
- Google Docs

## Learning Outcome
I learned the basic architecture of VPNs, how encrypted tunnels protect network traffic, the common types of VPNs, and why VPN encryption should not be confused with complete anonymity.

## Conclusion
VPNs are an important cybersecurity technology for protecting traffic across untrusted networks and enabling secure remote connectivity. They work best as one layer of a broader security strategy.

Note: This task documents conceptual learning. No live VPN configuration or practical testing is claimed.
# Task 19: Linux Security Basics (19 Oct 2026)

## Internship
**Organization:** Veda Technology  
**Track:** Cybersecurity  
**Task:** 19 — Linux Security Basics

## 1. Objective
To understand basic Linux security controls, including users, groups, file permissions, and ownership.

## 2. Tools Used
- JSLinux Online Linux Emulator
- Alpine Linux (x86_64 Console)
- Linux Terminal

## 3. Practical Performed
In this practical, I created a directory and file, modified file permissions, and checked user, group, and file ownership information.

## 4. Commands Used

### Create a directory and file
```bash
mkdir linux_security
cd linux_security
touch practical.txt
```

### Check file permissions
```bash
ls -l practical.txt
```

### Change permissions to 600
```bash
chmod 600 practical.txt
ls -l practical.txt
```
**Result:** The owner can read and write. Group and others have no permissions.

### Change permissions to 644
```bash
chmod 644 practical.txt
ls -l practical.txt
```
**Result:** The owner can read and write. Group and others can read the file.

### Change permissions to 700
```bash
chmod 700 practical.txt
ls -l practical.txt
```
**Result:** The owner has read, write, and execute permissions. Group and others have no permissions.

### Check user and group information
```bash
whoami
id
groups
```

### Check file details and ownership
```bash
stat practical.txt
```

## 5. Key Concepts Learned

- **chmod:** Changes file and directory permissions.
- **File Ownership:** Identifies the user and group associated with a file.
- **Read (r):** Allows reading file contents.
- **Write (w):** Allows modifying file contents.
- **Execute (x):** Allows executing a file when applicable.
- **Least Privilege:** Gives users only the permissions they need.

## 6. Results
The practical commands executed successfully in the JSLinux emulator. File permissions were changed to 600, 644, and 700. User and group information and file metadata were also checked.

The emulator session ran as the `root` user, as confirmed by the `whoami` and `id` commands.

## 7. Conclusion
This practical improved my understanding of Linux file permissions, ownership, and user/group information. I learned how to use basic Linux commands to inspect and manage file access permissions.

## Interview Questions
1. What is chmod?
>>chmod is a Linux command used to change file permissions.

2. What is file ownership?
>>It identifies the user and group that own a file.

3. What is the principle of least privilege?
>>Giving users only the permissions they need to do their work

## 8. Evidence
Attach the terminal screenshot showing the commands and their outputs as practical evidence.

# Task 20:Linux User Management (20 Oct 2026)

## Internship Practical — Veda Technology

### Objective
To understand Linux user account management, group creation, group membership, directory ownership, and access permissions.

### Tools Used
- JSLinux
- Alpine Linux v3.23
- Linux Terminal

### Practical Implementation

**1. Create a user**
```bash
adduser -D student1
```

**2. Verify the user**
```bash
id student1
```

**3. Create a group**
```bash
addgroup interns
```

**4. Add the user to the group**
```bash
addgroup student1 interns
```

**5. Create a practice directory**
```bash
mkdir -p /tmp/intern-lab
```

**6. Set directory ownership**
```bash
chown student1:interns /tmp/intern-lab
```

**7. Set directory permissions**
```bash
chmod 750 /tmp/intern-lab
```

**8. Verify directory permissions**
```bash
ls -ld /tmp/intern-lab
```

### Result
- Created the `student1` user account.
- Created the `interns` group.
- Added `student1` to the `interns` group.
- Created `/tmp/intern-lab` and assigned the appropriate owner and group.
- Applied permission mode `750`.

### Understanding Linux Permissions

Permission `750` means:
- **Owner (7):** Read, write, and execute.
- **Group (5):** Read and execute.
- **Others (0):** No permissions.

### Key Learnings
- Linux user and group management.
- Managing directory ownership.
- Applying file-system permissions.
- Understanding the principle of least privilege.

### Conclusion
This practical provided hands-on experience with basic Linux account administration and access control using a browser-based Alpine Linux environment.

# Task 22: Security Log Fundamentals (22 OCT 2026)

## 1. Introduction
Security Log Fundamentals is a basic cybersecurity task that helps us understand computer security logs and identify suspicious activities.

## 2. Objective
- To study common security logs.
- To identify important log fields such as timestamp, user, source IP address, and event type.
- To understand basic security event analysis.

## 3. Tools Used
- Windows Notepad (Text Editor)
- Sample authentication logs

## 4. Practical Steps
1. Created a text file named `security_logs.txt`.
2. Added sample authentication log entries to the file.
3. Identified the timestamp, user, source IP address, and event type in each entry.
4. Counted successful and failed login attempts.
5. Analysed repeated failed login attempts to identify potentially suspicious activity.
6. Prepared a report containing observations and a conclusion.

## 5. Sample Log Analysis
- Total log entries: 5
- Successful login attempts: 2
- Failed login attempts: 3
- User with repeated failed attempts: `admin`
- Source IP in the failed attempts: `203.0.113.25`

## 6. Observations
The sample logs show three failed login attempts for the admin account from the same source IP address. This pattern may indicate password guessing, but further investigation is needed to confirm whether an attack occurred.

## 7. Conclusion
This practical helped me understand how to read security logs, identify important fields, count login attempts, and recognise potentially suspicious activities. Security logs are useful for monitoring systems and investigating security incidents.

## 8. Files Included
- `security_logs.txt` – Contains sample authentication logs.
- `Security_Log_Fundamentals_Practical_Report.pdf` – Contains the practical report and screenshot evidence.
- `README.md` – Explains the task, tools, steps, and findings.

## 9. Interview Questions
**Q1. What is a security log?**  
A security log is a record of activities or events on a computer or network.

**Q2. What is a timestamp?**  
A timestamp shows the date and time when an event occurred.

**Q3. Why are security logs important?**  
They help identify suspicious activities, troubleshoot problems, and investigate security incidents.

**Note:** The log entries used in this practical are synthetic sample data created for educational purposes.

# Task 23: Authentication Log Analysis Using Microsoft Excel(23 Oct 2026)

## Project Overview
This project focuses on analyzing synthetic authentication logs using Microsoft Excel Online to identify successful logins, failed login attempts, and potentially suspicious login activity.

## Objective
- Count successful and failed login attempts.
- Analyze login records using Excel formulas.
- Identify IP addresses with repeated failed login attempts.
- Understand basic authentication monitoring in cybersecurity.

## Tools Used
- Microsoft Excel Online
- CSV dataset
- Excel formulas: `COUNTIF` and `COUNTIFS`

## Dataset Description
The dataset contains 20 synthetic login records with the following columns:

- **Timestamp:** Date and time of the login attempt.
- **Username:** Account name used for login.
- **Source IP:** IP address associated with the attempt.
- **Status:** Success or Failed.

## Methodology
1. Opened the CSV dataset in Excel Online.
2. Reviewed the login records and their status.
3. Used `COUNTIF` to count successful and failed logins.
4. Used `COUNTIF` and `COUNTIFS` to analyze a specific IP address.
5. Identified repeated failed login attempts for further investigation.

## Key Results
- Total login events: 20
- Successful logins: 7
- Failed logins: 13
- Failed attempts from IP `203.0.113.50`: 6

## Conclusion
The analysis identified repeated failed login attempts from one IP address. Such activity may indicate password guessing or other authentication issues and should be investigated further. Repeated failures alone do not prove that an attack occurred.

## Learning Outcomes
- Learned basic authentication log analysis.
- Practiced Excel formulas for security data analysis.
- Understood how failed login patterns can help identify potentially suspicious activity.
- Improved basic cybersecurity monitoring skills.

**Note:** This project uses synthetic data for educational purposes only.

## Task 24: Security Event Classification (23 Oct 2026)

## 📌 Project Overview
This project is a beginner-level cybersecurity practical focused on classifying security events as **Normal, Suspicious, or Potentially Malicious** using Microsoft Excel.

The goal is to understand basic security triage and learn how to identify unusual activities that may indicate potential security threats.

## 🎯 Objective
- Develop basic security event analysis skills.
- Classify sample security events into three categories.
- Document the reason behind each classification.
- Summarize the results using Excel.

## 🛠️ Tools Used
- Microsoft Excel
- Sample/Synthetic Security Event Logs

## 📋 Activities Performed
1. Reviewed 10 sample security events.
2. Classified each event based on its description.
3. Added reasons for the selected classifications.
4. Counted events in each category.
5. Prepared a conclusion summarizing the results.

## 📊 Results

| Classification | Number of Events |
|---|---:|
| Normal | 3 |
| Suspicious | 4 |
| Potentially Malicious | 3 |
| **Total** | **10** |

## 🔍 Examples of Security Events
- Successful login during normal hours
- Multiple failed login attempts
- Login from an unknown country
- Antivirus detecting known malware
- Many files encrypted suddenly
- Unknown program sending data externally

## 📚 Key Learnings
- Understood the basics of security triage.
- Learned to identify potentially suspicious activities.
- Practiced documenting reasons for security classifications.
- Learned how Excel can help organise and summarise security event data.

## ✅ Conclusion
This practical helped me understand how sample security events can be classified and reviewed using Microsoft Excel. It introduced me to basic cybersecurity analysis and the importance of investigating suspicious activities before reaching a final conclusion.

## ⚠️ Disclaimer
This project is for educational purposes only and uses sample security event descriptions. The classifications do not confirm that a real cyberattack occurred.

---
**Project:** Security Event Classification  
**Domain:** Cybersecurity  
**Level:** Beginner  
**Tool:** Microsoft Excel

# Task 25: Basic Incident Response  (25 Oct 2026)

## Overview
This project explains the basic stages of cybersecurity incident response and provides a practical checklist for handling security incidents.

## Objective
To understand incident response fundamentals and prepare a checklist for identifying, containing, and recovering from cybersecurity incidents.

## Topics Covered
- Preparation
- Detection and Analysis
- Containment
- Eradication
- Recovery
- Lessons Learned

## Tools Used
- Google Docs
- Basic cybersecurity knowledge

## Sample Scenario
A computer becomes infected after an employee opens a malicious email attachment.

The response includes detecting the infection, isolating the affected computer, investigating the incident, removing the malware, restoring the system, and documenting lessons learned.

## Deliverable
An incident response checklist covering all major stages of incident handling.

## Key Learnings
- Understood the importance of incident response.
- Learned how containment prevents an incident from spreading.
- Identified the steps required for safe recovery.
- Understood the importance of documentation and continuous improvement.

## Conclusion
A structured incident response process helps reduce the impact of cybersecurity incidents and improves an organization's security readiness.

# Task 26:Data Privacy Basics – Cybersecurity Practical (26 Oct 2026)

## Overview
This project focuses on identifying different types of information and recommending suitable protection measures to maintain data privacy and security.

## Objective
To understand data classification and learn how to protect public, internal, confidential, and sensitive information.

## Tools Used
- Google Sheets

## Practical Tasks
1. Created a data classification table.
2. Classified information into public, internal, confidential, and sensitive categories.
3. Identified potential risks if information is exposed.
4. Recommended protection measures for each data item.
5. Prepared a conclusion on the importance of data privacy.

## Data Classification Examples

| Data Item | Classification | Protection Measure |
|---|---|---|
| Customer Name | Confidential | Restrict access |
| Email Address | Confidential | Use access controls |
| Phone Number | Sensitive | Mask phone numbers |
| Password | Sensitive | Store salted password hashes |
| Company Policy | Internal | Allow authorized access only |
| Public Website URL | Public | Perform regular security checks |
| Payment Card Details | Sensitive | Avoid unnecessary storage |

## Key Concepts Learned
- Data classification
- Sensitive information protection
- Access control
- Encryption
- Data minimization
- Data leakage prevention

## Conclusion
Data classification helps organizations identify and protect information according to its sensitivity. Applying appropriate security measures such as encryption, access control, and data minimization reduces the risk of data leakage, identity theft, and unauthorized access.

## Disclaimer
All examples used in this practical are illustrative or synthetic and should not be treated as real customer information.
