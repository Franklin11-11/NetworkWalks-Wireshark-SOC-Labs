# Lab 04: Follow TCP Stream — Part 1

## Objective

Reconstruct a TCP conversation in Wireshark and inspect the application data exchanged between two endpoints.

## Tools

* Wireshark
* Kali Linux
* TCP stream analysis

## Investigation Findings

| Item                           | Observation     |
| ------------------------------ | --------------- |
| Packets captured               | 246             |
| TCP port used by the chat      | 5000            |
| Client that initiated the chat | `192.168.10.45` |
| TCP stream index               | 5               |

## Investigation Method

1. Examined the captured packets in Wireshark.
2. Identified the TCP conversation using port and endpoint information.
3. Followed the relevant TCP stream to reconstruct the application-level exchange.
4. Reviewed the reconstructed conversation for information disclosed in transit.

## Security Observations

The reconstructed chat contained internal business information, including references to a finance drive, a help-desk ticket, and passwords.

Sensitive values have intentionally been omitted from this public report.

## Security Recommendations

* Do not transmit passwords through unencrypted chat or network services.
* Use encrypted communication channels and secure authentication.
* Avoid sharing Wi-Fi credentials or temporary passwords in plain text.
* Rotate credentials that may have been exposed.
* Restrict access to internal systems and sensitive business information.

## Evidence

Screenshots have not yet been added. The stream details and observations should be supported with sanitized screenshots where available.

## Learning Outcome

This exercise demonstrates how following a TCP stream can reconstruct application conversations and expose sensitive information that may not be obvious from individual packets.

