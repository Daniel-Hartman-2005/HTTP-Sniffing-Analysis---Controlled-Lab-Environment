# HTTP Sniffing Analysis – Controlled Lab Environment

## Overview
This project demonstrates HTTP traffic analysis in a controlled lab environment. 
The objective is to observe how unencrypted HTTP communication can expose sensitive 
information such as credentials when captured using packet analysis tools.

## Lab Environment
- Attacker Machine: Kali Linux
- Target Machine: Metasploitable2 (DVWA)
- Tool: Wireshark
- Network Type: Isolated / Host-only Network

## Methodology
1. A login request was performed over HTTP.
2. Network traffic was captured using Wireshark.
3. HTTP packets were filtered and analyzed.
4. Sensitive information was identified in plaintext.

## Findings
- HTTP traffic is transmitted without encryption.
- Login credentials can be captured in plaintext.
- This demonstrates why HTTP is insecure for sensitive communication.

## Evidence
Screenshots below show captured HTTP packets and credential exposure during analysis.

## Disclaimer
This project was conducted strictly in a controlled lab environment for educational purposes only.
