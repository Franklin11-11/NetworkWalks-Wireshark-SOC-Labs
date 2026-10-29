# Lab 05: Follow TCP Stream — Part 2

## Objective

Analyze HTTP traffic in Wireshark, inspect web requests and server responses, and investigate content exchanged between a client and web server.

## Tools

* Wireshark
* Kali Linux
* HTTP display filters
* TCP stream reconstruction

## Investigation Findings

Several HTTP request paths were observed during the investigation, including:

* `/index.html`
* `/about.html`
* `/staff.html`
* `/contact.html`
* `/news.html`
* `/download/report.txt`

The root path `/` returned an HTTP `200 OK` response containing a page identifying the site as a company intranet.

The `/staff.html` request also returned status code `200`.

## Investigation Method

1. Inspected HTTP requests and responses in Wireshark.
2. Reviewed requested paths and response status codes.
3. Followed relevant TCP streams to inspect application-level content.
4. Examined the response containing the downloadable text report.
5. Investigated whether HTML content contained a hidden note.

## Findings Requiring Further Verification

The hidden note's complete contents, the backup server IP address, and the author of the downloaded report have not been confirmed in this report.

These details should be added only after reviewing the original packet capture.

## Security Recommendations

* Avoid storing sensitive operational notes in publicly accessible web content.
* Review HTML source and comments for accidentally exposed internal information.
* Restrict access to internal documents and downloadable files.
* Apply appropriate authentication and access controls to intranet resources.
* Use HTTPS to protect web traffic in transit.

## Evidence

Screenshots have not yet been added. Add sanitized screenshots of relevant HTTP requests, responses, and stream contents when available.

## Learning Outcome

This exercise demonstrates how HTTP request paths, response codes, and reconstructed TCP streams can help an analyst investigate web traffic and identify potentially exposed information.
