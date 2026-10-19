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
