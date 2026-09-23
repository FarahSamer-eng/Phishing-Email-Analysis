# Phishing Indicators

## Overview

This file documents the main indicators identified during the phishing email analysis.

## Indicators Identified

| Indicator              | Example / Evidence                               | Security Concern                       |
| ---------------------- | ------------------------------------------------ | -------------------------------------- |
| Spoofed Sender         | Fake sender addresses and display names          | Sender identity deception              |
| Brand Impersonation    | PayPal, Netflix, Apple, DHL, Microsoft           | Increased user trust                   |
| Artificial Urgency     | Account, billing, shipment, or document warnings | Pressure to act quickly                |
| Suspicious Links       | Deceptive hyperlinks and tracking links          | Redirection to malicious destinations  |
| URL Shortening         | Shortened URLs hiding the final destination      | Destination obfuscation                |
| URL Redirection        | Multiple redirect stages                         | Hiding phishing infrastructure         |
| Tracking Pixel         | Embedded tracking image                          | User activity tracking                 |
| Credential Harvesting  | Fake Microsoft/Outlook login portal              | Credential theft                       |
| Suspicious Attachments | `.dot`, `.xlsx`, and PDF files                   | Potential malware or phishing delivery |
| BCC Usage              | Recipients hidden using BCC                      | Suspicious bulk email behavior         |
| Executable Reference   | `regasms.exe`                                    | Potential malicious payload            |

## Brand Impersonation

Several phishing samples attempted to imitate well-known organizations, including:

* PayPal
* OneDrive
* Adobe
* Microsoft/Outlook
* Netflix
* Apple
* DHL

Brand impersonation was used to make the messages appear trustworthy.

## Link-Based Indicators

The analyzed emails contained several suspicious link techniques:

* Shortened URLs
* Deceptive hyperlinks
* Redirect chains
* Links that did not match the expected legitimate domain
* Links leading to credential-harvesting pages

## Attachment-Based Indicators

Suspicious attachments were identified in several samples.

Examples included:

* PDF attachment
* `.dot` document
* `.xlsx` spreadsheet

Attachments can be used to deliver malicious content or redirect users to phishing websites.

## Credential Harvesting

One of the analyzed phishing emails used multiple redirects to reach a fake Outlook login portal.

The purpose of the fraudulent portal was to capture user credentials.

**Attack Type:** Credential Harvesting

## Malicious Payload

The DHL phishing sample contained an Excel attachment that referenced the executable:

`regasms.exe`

This represents a significant indicator of potentially malicious activity.

## Recommended Actions

* Verify sender addresses independently.
* Hover over links before clicking them.
* Inspect suspicious URLs.
* Avoid shortened links from unexpected messages.
* Do not open unexpected attachments.
* Verify requests through official websites or known contact methods.
* Report suspicious emails to the security team.

## Assessment Context

All indicators documented in this file were identified in a controlled TryHackMe training environment for educational purposes.
