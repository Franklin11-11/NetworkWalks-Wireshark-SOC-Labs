# NetworkWalks Wireshark SOC Labs

## Project Overview

This repository documents my hands-on network traffic analysis and security investigation exercises using Wireshark. The labs focus on examining packet captures, investigating suspicious network activity, identifying exposed information, and understanding network-based attack indicators.

The project demonstrates practical skills relevant to Security Operations Center (SOC) analysis, network security monitoring, and incident investigation.

## Objectives

* Analyze packet captures using Wireshark.
* Identify suspicious IP addresses and network communication patterns.
* Inspect TCP streams and HTTP requests.
* Understand the risks of transmitting credentials over unencrypted protocols.
* Investigate FTP authentication failures and potential brute-force activity.
* Examine SIP and RTP traffic associated with VoIP communications.
* Document investigation methods, observations, and security recommendations.

## Tools and Technologies

* Wireshark
* Kali Linux
* Network packet analysis
* TCP/IP
* HTTP
* FTP
* SIP and RTP
* Git and GitHub

## Labs

| Lab | Investigation                 | Key Skills                                                     |
| --- | ----------------------------- | -------------------------------------------------------------- |
| 03  | Identify the Attacker's IP    | IP address investigation and traffic analysis                  |
| 04  | Follow TCP Stream — Part 1    | TCP stream reconstruction and application-data inspection      |
| 05  | Follow TCP Stream — Part 2    | HTTP response analysis and web-content inspection              |
| 06  | HTTP Plain-Text Credentials   | HTTP POST analysis and credential-exposure investigation       |
| 07  | FTP Brute-Force Investigation | Authentication-failure analysis and suspicious login detection |
| 08  | VoIP Traffic Investigation    | SIP signaling and RTP media-traffic analysis                   |

Detailed notes and supporting screenshots will be added to each lab directory as the evidence is reviewed.

## Investigation Methodology

My general workflow includes:

1. Open the relevant packet capture in Wireshark.
2. Apply protocol-specific display filters.
3. Identify relevant endpoints, packets, and communication sessions.
4. Inspect packet details and reconstruct streams where appropriate.
5. Record findings supported by packet-level evidence.
6. Explain the security implications.
7. Recommend defensive measures where applicable.

## Key Security Lessons

These exercises demonstrate why organizations should:

* Use encrypted protocols such as HTTPS instead of transmitting sensitive information over plain HTTP.
* Monitor repeated authentication failures and investigate suspicious login patterns.
* Avoid exposing FTP services and use secure alternatives such as SFTP or FTPS where appropriate.
* Review network traffic for suspicious connections and unexpected application behavior.
* Investigate VoIP signaling and media traffic while respecting privacy and authorization requirements.
* Maintain clear investigation notes and preserve relevant evidence.

## Scope and Ethics

These exercises were conducted for educational and defensive security-learning purposes using designated lab materials.

Findings should be reported only when supported by packet-capture evidence. Sensitive credentials, personal information, and private communications should not be published in this repository.

## Future Improvements

* Add sanitized screenshots of relevant Wireshark filters and packet details.
* Document verified findings for each lab.
* Include investigation reports and defensive recommendations.
* Expand the portfolio with additional network security and incident-response exercises.

## Author

**Franklin Chukwuemeka**

GitHub: [Franklin11-11](https://github.com/Franklin11-11)
