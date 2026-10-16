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
