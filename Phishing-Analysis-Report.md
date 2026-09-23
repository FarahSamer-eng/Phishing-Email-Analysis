# Phishing Email Analysis Report

## 1. Assessment Overview

This assessment was conducted in a controlled TryHackMe training environment to analyze multiple phishing email samples.

The investigation focused on identifying phishing indicators, analyzing sender information, suspicious links, URL redirection, tracking pixels, credential harvesting, and malicious attachments.

## 2. Environment

| Item            | Details                         |
| --------------- | ------------------------------- |
| Platform        | TryHackMe                       |
| Room            | Phishing Emails in Action       |
| Assessment Type | Phishing Email Analysis         |
| Environment     | Controlled Training Environment |

## 3. Analysis Methodology

The phishing emails were analyzed using the following methods:

* Sender and display name inspection
* Email content analysis
* Email source and HTML inspection
* Hyperlink analysis
* URL redirection investigation
* Tracking pixel identification
* Attachment analysis
* Identification of social engineering techniques

## 4. Email Analysis

### 4.1 Fake PayPal Transaction

The email impersonated PayPal and presented a fraudulent transaction notification.

**Identified indicators:**

* Spoofed sender information
* PayPal brand impersonation
* Suspicious transaction details
* URL shortening
* Suspicious link leading to an external destination

**Merchant shown in the email:** Walmart

---

### 4.2 Fake Shipping Notification

The email impersonated a distribution center and attempted to convince the recipient to follow a fake tracking link.

**Identified indicators:**

* Spoofed sender address
* Fake tracking number
* Link manipulation
* Tracking pixel
* Suspicious redirect link

---

### 4.3 Fake Document Notification

The email used multiple trusted brands and redirects to lead the victim to a fraudulent login page.

**Identified indicators:**

* Artificial urgency
* OneDrive impersonation
* Adobe impersonation
* Microsoft/Outlook impersonation
* Multi-stage URL redirection
* Fake login portal

**Attack type:**

Credential Harvesting

---

### 4.4 Fake Netflix Billing Notification

The email impersonated Netflix and claimed that there was an issue with the recipient's billing information.

**Identified indicators:**

* Spoofed display name
* Netflix brand impersonation
* Artificial urgency
* Poor grammar and spelling
* Suspicious PDF attachment
* Embedded malicious link

---

### 4.5 Fake Apple Purchase Notification

The email impersonated Apple and contained a suspicious document attachment.

**Identified indicators:**

* Spoofed sender display name
* Apple brand impersonation
* BCC usage
* Blank email body
* Suspicious document attachment
* Embedded link leading to a phishing site

**Attachment extension:**

`.dot`

**BCC:** Blind Carbon Copy

---

### 4.6 Fake DHL Shipment Notification

The email impersonated DHL and contained a suspicious Excel attachment.

**Identified indicators:**

* Spoofed display name
* DHL brand impersonation
* Suspicious `.xlsx` attachment
* Inconsistent domain and geographic information
* Inconsistent document language
* Malicious executable reference

**Executable identified:**

`regasms.exe`

## 5. Common Phishing Techniques

| Technique             | Description                                                 |
| --------------------- | ----------------------------------------------------------- |
| Sender Spoofing       | Manipulating sender information to appear legitimate        |
| Brand Impersonation   | Using trusted companies to increase credibility             |
| Artificial Urgency    | Creating pressure to make the victim act quickly            |
| URL Shortening        | Hiding the final destination of a malicious link            |
| Link Manipulation     | Using deceptive hyperlinks                                  |
| URL Redirection       | Redirecting victims through multiple destinations           |
| Tracking Pixels       | Tracking whether an email has been opened                   |
| Credential Harvesting | Capturing credentials through fake login pages              |
| Malicious Attachments | Using documents to deliver or redirect to malicious content |

## 6. Risk Considerations

The analyzed phishing techniques could lead to:

* Credential theft
* Unauthorized account access
* Malware infection
* Information disclosure
* User tracking
* Further compromise of systems or accounts

## 7. Recommended Security Controls

* Verify the actual sender address before interacting with an email.
* Avoid clicking unexpected links.
* Inspect suspicious URLs before opening them.
* Be cautious with shortened or redirected URLs.
* Do not open unexpected attachments.
* Verify billing, shipping, and transaction notifications through official channels.
* Never enter credentials into suspicious login portals.
* Report suspected phishing emails to the security team.

## 8. Conclusion

The assessment demonstrated how phishing emails use social engineering, spoofing, malicious links, redirects, tracking mechanisms, credential harvesting, and attachments to deceive users.

Analyzing sender information, email content, URLs, source code, and attachments can help identify phishing attempts before they result in compromise.

## Disclaimer

This assessment was performed in a controlled TryHackMe training environment for educational purposes. No production systems or personal accounts were targeted.
