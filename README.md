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

