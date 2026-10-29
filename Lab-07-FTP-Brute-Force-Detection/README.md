# Lab 07: FTP Brute-Force Investigation

## Objective

Analyze FTP traffic in Wireshark to identify repeated authentication failures and investigate indicators of a possible brute-force attack.

## Tools

* Wireshark
* Kali Linux
* FTP protocol analysis
* Network packet inspection

## Investigation Findings

| Item                                        | Observation     |
| ------------------------------------------- | --------------- |
| Protocol                                    | FTP             |
| FTP server IP                               | `192.168.10.20` |
| Suspected source IP                         | `192.168.10.66` |
| Repeatedly attempted username               | `admin`         |
| Failed authentication response              | `530`           |
| Successful authentication response observed | `230`           |

The capture contained repeated login attempts involving the username `admin`. FTP response code `530` indicated unsuccessful authentication, while response code `230` indicated that a login was successful.

The total number of failed attempts and the exact credentials associated with the successful login have not been verified for this report.

## Investigation Method

1. Filtered FTP traffic in Wireshark.
2. Examined authentication requests and server responses.
3. Identified the source and destination IP addresses.
4. Reviewed repeated authentication failures and relevant response codes.
5. Looked for evidence of a subsequent successful login.

## Security Impact

FTP does not protect credentials in transit by default. Depending on the connection and configuration, usernames, passwords, and transferred data may be exposed to network observers.

Repeated authentication failures followed by a successful login may indicate a password-guessing attack, although the activity should be validated before classifying it as malicious.

## Security Recommendations

* Replace unencrypted FTP with SFTP or appropriately configured FTPS.
* Disable unused FTP services.
* Enforce strong, unique passwords and multi-factor authentication where supported.
* Monitor repeated login failures and unusual authentication patterns.
* Apply rate limiting or temporary lockout policies where appropriate.
* Investigate successful logins that follow repeated failures.
* Review server logs and correlate the activity with other security telemetry.

## Evidence

Screenshots have not yet been added. Add sanitized screenshots of relevant FTP requests, response codes, and endpoint information.

Do not publish recovered passwords or other sensitive authentication data.

## Learning Outcome

This exercise demonstrates how protocol-level analysis can help identify suspicious authentication patterns and why repeated failures followed by a successful login warrant further investigation.
