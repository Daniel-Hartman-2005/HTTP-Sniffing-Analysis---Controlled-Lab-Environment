<h1>HTTP Sniffing Analysis – Controlled Lab Environment</h1>

## Overview
This project demonstrates HTTP traffic analysis in a controlled lab environment. 
The objective is to observe how unencrypted HTTP communication can expose sensitive 
information such as credentials when captured using packet analysis tools.

## Disclaimer
This project was conducted strictly in a controlled lab environment for educational purposes only.

## Lab Environment
- Attacker Machine: Kali Linux
- Target Machine: Metasploitable2 (DVWA)
- Tool: Wireshark
- Network Type: Isolated / Host-only Network / NAT Network

## Analysis Flow
1. DVWA Login Page over HTTP <br>
This image shows the login page of Damn Vulnerable Web Application (DVWA) accessed over the HTTP protocol, which is not encrypted. Because the connection is unsecured, any data entered on this page—such as usernames, passwords, or session information—can potentially be captured and analyzed through network traffic sniffing.

2. Credentials Leak <br>
HTTP communication is not encrypted, the login credentials can be clearly observed within the captured traffic. This demonstrates how sensitive information can be exposed when applications rely on unsecured HTTP connections instead of HTTPS.

3. HTTPS Traffic <br>
The screenshot is used to illustrate the importance of encrypted communication and how security professionals analyze network traffic to identify potential data exposure risks in web applications.

## Findings
- HTTP traffic is transmitted without encryption.
- Login credentials can be captured in plaintext.
- This demonstrates why HTTP is insecure for sensitive communication.

## Mitigation
To mitigate the risks shown in this project, HTTP communication should be avoided for sensitive data and replaced with HTTPS to ensure encryption in transit. Secure session handling, proper network segmentation, and disabling unnecessary insecure services can significantly reduce the risk of credential exposure. Regular security testing also helps identify and prevent misconfigurations early.


