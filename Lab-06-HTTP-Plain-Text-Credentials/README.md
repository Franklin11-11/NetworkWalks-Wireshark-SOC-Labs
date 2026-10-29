# Lab 06: HTTP Plain-Text Credentials

## Objective

Investigate HTTP login traffic in Wireshark to determine how credentials submitted through an unencrypted web form can be exposed during network transmission.

## Tools

* Wireshark
* Kali Linux
* HTTP protocol analysis
* TCP stream inspection

## Investigation Findings

| Item                       | Observation     |
| -------------------------- | --------------- |
| Application protocol       | HTTP            |
| HTTP method                | POST            |
| Login endpoint             | `/login`        |
| Client IP                  | `192.168.10.45` |
| Server IP                  | `192.168.10.20` |
| Observed login submissions | 2               |

The packet capture contained HTTP form submissions to the login endpoint. The request details indicated that the form used URL-encoded data.

Credential values have intentionally been excluded from this public report.

## Investigation Method

1. Applied HTTP-related display filters in Wireshark.
2. Located POST requests directed to `/login`.
3. Inspected packet details to identify the form encoding.
4. Reviewed the requests to determine whether login information was transmitted without transport encryption.
5. Compared the observed submissions in the packet capture.

## Security Impact

Credentials submitted through unencrypted HTTP may be readable by parties able to capture the relevant network traffic. This can expose user accounts to credential theft and unauthorized access.

## Security Recommendations

* Enforce HTTPS using properly configured TLS.
* Redirect HTTP requests to HTTPS and enable HTTP Strict Transport Security where appropriate.
* Never submit credentials through unencrypted login forms.
* Use multi-factor authentication as an additional security control.
* Monitor for suspicious authentication activity and rotate credentials if exposure is suspected.

## Evidence

Screenshots have not yet been added. Add sanitized screenshots showing the HTTP method, endpoint, and form-encoding details. Do not publish usernames, passwords, session cookies, or authentication tokens.

## Learning Outcome

This exercise demonstrates how Wireshark can reveal the security weaknesses of unencrypted login traffic and why TLS is essential for protecting credentials in transit.
