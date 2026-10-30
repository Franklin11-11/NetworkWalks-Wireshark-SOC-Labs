# Wireshark Investigation Evidence

This directory contains screenshots documenting practical network traffic analysis using Wireshark.

The screenshots demonstrate packet inspection, TCP connection analysis, HTTP request and response examination, and TCP stream reconstruction.

## Evidence Files

### 02 — HTTP Request and Response

**File:** `02-http-request-response.png`

Shows an HTTP GET request from a local client to a Python HTTP server, alongside the server's successful HTTP 200 OK response.

**Skills demonstrated:**

* HTTP traffic inspection
* Request and response identification
* Client-server communication analysis

### 03 — TCP Three-Way Handshake

**File:** `03-tcp-three-way-handshake.png`

Shows the three stages of TCP connection establishment:

1. SYN
2. SYN-ACK
3. ACK

**Skills demonstrated:**

* TCP connection analysis
* TCP flag identification
* Client-server connection establishment

### 04 — Follow TCP Stream

**File:** `04-follow-tcp-stream.png`

Shows a reconstructed TCP conversation containing an HTTP request and the corresponding server response.

**Skills demonstrated:**

* TCP stream reconstruction
* Application-layer traffic analysis
* HTTP communication inspection

### 05 — HTTP Packet Bytes

**File:** `05-http-packet-bytes.png`

Shows the hexadecimal and ASCII representation of an HTTP request at packet level.

**Skills demonstrated:**

* Packet-level inspection
* Hexadecimal and ASCII interpretation
* HTTP header identification

## Lab Environment

The screenshots in this collection were generated using:

* Operating System: Kali Linux
* Virtualisation: Oracle VirtualBox
* Packet Analysis Tool: Wireshark 4.6.4
* Network Interface: Loopback (`lo`)
* Client: curl
* Server: Python SimpleHTTPServer
* Server Address: `127.0.0.1:8000`

## Scope and Accuracy

These four screenshots document a controlled local network traffic demonstration. They are supplementary portfolio evidence and are not represented as screenshots from the original NetworkWalks exercises or their packet captures.

No external systems were targeted during this demonstration.

