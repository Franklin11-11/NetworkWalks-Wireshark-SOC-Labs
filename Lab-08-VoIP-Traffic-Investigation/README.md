# Lab 08: VoIP Traffic Investigation

## Objective

Analyze Voice over IP (VoIP) network traffic in Wireshark to identify call-signaling protocols, examine media-traffic characteristics, and understand the security implications of network-based voice communications.

## Tools

* Wireshark
* Kali Linux
* SIP protocol analysis
* RTP traffic analysis

## Investigation Findings

| Item                    | Observation |
| ----------------------- | ----------- |
| Call-signaling protocol | SIP         |
| Voice-media protocol    | RTP         |

The packet capture contained SIP signaling traffic used to establish and manage a VoIP call, as well as RTP traffic associated with voice media.

The caller extension, answering party, negotiated codec, and requested card-number detail have not been verified in this report.

## Investigation Method

1. Examined the packet capture for SIP signaling.
2. Identified call-related signaling messages.
3. Inspected RTP traffic associated with the call.
4. Reviewed protocol fields that can help identify call participants and media characteristics.
5. Recorded the findings that could be verified from the available investigation notes.

## Security Considerations

VoIP security depends on the configuration of signaling, media transport, and the surrounding network. Unprotected signaling or media may expose call metadata or voice content to parties with access to the traffic.

Sensitive conversations and personal or payment-card information should not be extracted or published unnecessarily.

## Security Recommendations

* Use appropriate signaling protection, such as SIP over TLS where supported.
* Protect voice media using SRTP where supported.
* Restrict access to VoIP infrastructure and management interfaces.
* Monitor unusual call patterns and unexpected signaling activity.
* Apply network segmentation and access controls to voice systems.
* Handle captured communications in accordance with privacy and authorization requirements.

## Evidence

Screenshots have not yet been added. Add sanitized screenshots showing SIP signaling and RTP packet details, with sensitive information removed.

## Learning Outcome

This exercise demonstrates how Wireshark can distinguish VoIP signaling from media traffic and help analysts investigate communication protocols while respecting privacy and authorization requirements.
