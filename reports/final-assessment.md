# Final Assessment: Wireshark SOC Labs

## Overview

This project involved a series of hands-on network traffic analysis exercises using Wireshark. The exercises covered TCP stream reconstruction, HTTP traffic inspection, authentication analysis, and VoIP protocol investigation.

The objective was to develop practical skills in examining packet captures, identifying security weaknesses, and documenting findings in a structured format.

## Skills Practiced

* Packet inspection and protocol analysis
* IP address and endpoint investigation
* TCP stream reconstruction
* HTTP request and response analysis
* Identification of potential credential exposure
* FTP authentication-failure investigation
* SIP signaling and RTP media-traffic analysis
* Security reporting and defensive recommendations

## Summary of Exercises

| Lab | Focus                      | Key Learning                                                            |
| --- | -------------------------- | ----------------------------------------------------------------------- |
| 03  | Attacker IP identification | Investigating network endpoints and suspicious traffic                  |
| 04  | TCP stream reconstruction  | Reconstructing application conversations from packets                   |
| 05  | HTTP stream analysis       | Examining web paths, responses, and exposed content                     |
| 06  | HTTP credentials           | Understanding risks associated with unencrypted login traffic           |
| 07  | FTP authentication         | Investigating repeated failures and possible password-guessing activity |
| 08  | VoIP traffic               | Distinguishing SIP signaling from RTP media traffic                     |

## Security Recommendations

Based on the topics covered in these exercises:

1. Encrypt sensitive communications in transit.
2. Investigate repeated authentication failures and unusual login patterns.
3. Restrict access to internal services and sensitive resources.
4. Review network traffic and authentication logs for suspicious activity.
5. Preserve investigation evidence and document findings accurately.
6. Avoid exposing credentials, private communications, or personal information in public reports.

## Limitations

Some lab-specific answers and supporting screenshots remain unverified or unavailable. The individual reports identify these gaps rather than presenting unconfirmed details as established facts.

The findings documented in this repository should be interpreted within the scope of the available lab evidence.

## Conclusion

These exercises provided practical exposure to Wireshark-based network investigation and common network security concerns. They strengthened my understanding of packet-level analysis, protocol behavior, authentication risks, and security reporting.

Further practice will focus on improving evidence collection, documenting verified findings, and developing repeatable investigation workflows relevant to SOC operations.
