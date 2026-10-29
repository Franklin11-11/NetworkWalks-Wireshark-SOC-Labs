
# Wireshark SOC Investigation Labs

Hands-on network traffic analysis and security investigation exercises using Wireshark. This portfolio demonstrates practical skills in packet analysis, TCP stream reconstruction, HTTP security assessment, FTP authentication monitoring, and VoIP traffic investigation.

## About This Project

This project documents my hands-on practice analysing network traffic from a Security Operations Center (SOC) perspective. I used Wireshark to inspect packet captures, identify suspicious activity, investigate application-layer protocols, and document security findings.

**Focus areas:** Network security monitoring | Packet analysis | Protocol investigation | Authentication security | Incident documentation

## Tools and Technologies

- **Wireshark** — packet capture analysis and protocol inspection
- **Display filters** — targeted traffic investigation
- **TCP stream following** — reconstruction of application conversations
- **HTTP and FTP analysis** — investigation of insecure communications and authentication activity
- **SIP/RTP analysis** — VoIP signalling and media-traffic investigation

## Lab Investigations

| Lab | Investigation | Skills Practised |
|---|---|---|
| 03 | Identify an Attacker's IP | Traffic inspection and source-IP investigation |
| 04 | Follow TCP Stream — Part 1 | TCP stream reconstruction and conversation analysis |
| 05 | Follow TCP Stream — Part 2 | HTTP response inspection and web-content investigation |
| 06 | HTTP Plain-Text Credentials | HTTP POST analysis and insecure authentication detection |
| 07 | FTP Brute-Force Detection | FTP login monitoring and repeated authentication-failure investigation |
| 08 | VoIP Traffic Investigation | SIP signalling and RTP media-traffic analysis |

Open each lab folder to read its investigation notes, observations, limitations, and security lessons.

## Selected Findings

### HTTP Authentication
- Identified HTTP POST requests to a login endpoint.
- Observed client-to-server traffic between `192.168.10.45` and `192.168.10.20`.
- Documented the risk of transmitting authentication data over unencrypted HTTP.
- Sensitive credential values are intentionally excluded from this public portfolio.

### FTP Authentication Monitoring
- Investigated repeated FTP login attempts involving the `admin` username.
- Observed FTP response codes associated with failed and successful authentication.
- Documented how repeated failures followed by a successful login can warrant further investigation.
- Findings should be validated against the complete packet capture before drawing conclusions about compromise.

### TCP and Application-Protocol Analysis
- Used TCP stream reconstruction to examine application conversations.
- Inspected HTTP paths and server responses.
- Reviewed SIP signalling and RTP traffic as part of a VoIP investigation.

## Investigation Methodology

For each exercise, I aimed to:

1. Identify the relevant hosts and protocols.
2. Apply targeted Wireshark display filters.
3. Inspect packet details and reconstruct streams where appropriate.
4. Record observable evidence and distinguish verified findings from unanswered questions.
5. Document security implications and recommended follow-up actions.

## Security Lessons

- Plain-text protocols can expose sensitive information to anyone able to capture the traffic.
- Repeated authentication failures followed by success deserve contextual investigation.
- Packet evidence should be validated before classifying an event as malicious.
- Public reports should avoid exposing passwords, personal information, or private communications.
- Effective security analysis requires clear documentation of both findings and limitations.

## Project Structure

```text
.
├── README.md
├── Lab-03-Identify-Attackers-IP/
├── Lab-04-Follow-TCP-Stream-Part-1/
├── Lab-05-Follow-TCP-Stream-Part-2/
├── Lab-06-HTTP-Plain-Text-Credentials/
├── Lab-07-FTP-Brute-Force-Detection/
├── Lab-08-VoIP-Traffic-Investigation/
└── reports/
    └── final-assessment.md
````

## Professional Development

These exercises support my continued development in:

* Security Operations Center (SOC) analysis
* Network traffic analysis
* Security event investigation
* Authentication and protocol security
* Technical report writing

## Ethics and Scope

These exercises were performed for educational purposes using lab-provided traffic. Findings are limited to the evidence documented in each report. Sensitive credentials and private communications are not published.

## Author

**Franklin Chukwuemeka**

* GitHub: [Franklin11-11](https://github.com/Franklin11-11)

