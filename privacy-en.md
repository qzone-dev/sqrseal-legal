---
title: SQRSeal Privacy Policy
---
<style>
body { background: #ffffff; color: #1a1a2e; font-family: system-ui, sans-serif; max-width: 800px; margin: 0 auto; padding: 2rem 1.5rem; line-height: 1.7; }
h1,h2,h3 { color: #0f172a; }
a { color: #0ED797; }
</style>
**Last updated:** June 2026  
**Effective date:** June 2026

---

## 1. Introduction

SQRSeal ("the app", "we", "us") is a URL and QR code security analysis application designed to protect users in the digital world. This Privacy Policy explains what data is collected when you use our application, how it is used, and your rights.

By using the application, you agree to this policy. If you do not agree, please do not use the application.

---

## 2. Data We Collect

### 2.1 Automatically Collected Data

**Anonymous Device ID**
- A random device identifier is generated on the app's first launch.
- This ID is stored on your device and transmitted to our Supabase servers.
- It is not linked to your name, email address, phone number, or any other personal identifying information.
- If you reinstall the app, a new ID is generated.

**Queried URL and Domain Information**
- The domain portion of URLs you enter, scan, or that are captured from your clipboard is transmitted to our servers for security analysis.
- URLs are processed solely to detect security threats.
- We recommend avoiding queries containing sensitive personal information.

**Query Statistics**
- Total query count, threat detection results, and scan source (manual, QR, OCR, clipboard) are recorded.
- This data is used solely to display your personal statistics within the app.

**Technical Performance Data**
- Response time (ms), cache usage, and network connection information are collected.
- This data is used to improve app performance and cannot be used to identify you.

**App Events**
- In-app events such as opening a link and OCR scanning are recorded anonymously.
- This data is used for product development purposes.

### 2.2 Data We Do NOT Collect

The following data is **never collected:**
- Name, surname, email address, phone number
- Location data
- Photos or camera footage (images uploaded during OCR analysis are automatically deleted after processing)
- Clipboard content (only checked for URL presence; if not a URL, no action is taken)
- Social media or account credentials

---

## 3. How We Use Your Data

Collected data is used exclusively for the following purposes:

| Purpose | Data |
|---------|------|
| Providing URL security analysis | Domain information |
| Displaying personal query history | Query records |
| Measuring app performance | Technical metrics |
| Detecting and fixing errors | Crash reports |
| Making product development decisions | Anonymous usage statistics |

Your data is never sold, rented, or shared with third parties for commercial purposes.

---

## 4. Third-Party Services

SQRSeal uses the following third-party services to perform security analysis. Each service is subject to its own privacy policy.

### 4.1 Google Web Risk API
- **Purpose:** Checking URLs against known threat databases
- **Data transmitted:** Queried URL
- **Privacy policy:** https://policies.google.com/privacy

### 4.2 URLScan.io
- **Purpose:** In-depth security scanning of URLs
- **Data transmitted:** Queried URL
- **Privacy policy:** https://urlscan.io/about/#privacy

### 4.3 Supabase
- **Purpose:** Database and server infrastructure
- **Data transmitted:** Anonymous device ID, query records
- **Data center:** European Union
- **Privacy policy:** https://supabase.com/privacy

### 4.4 Sentry
- **Purpose:** Application error tracking and crash reporting
- **Data transmitted:** Error information, device type, OS version
- **Personal data:** Not transmitted (`sendDefaultPii: false`)
- **Privacy policy:** https://sentry.io/privacy/

### 4.5 USOM (Turkish National Cyber Incident Response Center)
- **Purpose:** Receiving Turkey-specific threat data
- **Data transmitted:** None (data is only received, not sent)
- **Institution:** Information and Communication Technologies Authority of Turkey

### 4.6 Other Threat Intelligence Sources
Open-source threat intelligence databases including URLhaus, OpenPhish, and BOTVRIJ are automatically queried. No user data is transmitted in this process.

---

## 5. Clipboard Access

When the "Link Capturing" feature is enabled, SQRSeal periodically monitors your clipboard. This feature:

- Only checks whether the clipboard content contains a URL.
- If a URL is detected, initiates a security analysis.
- If not a URL, the clipboard content is neither processed nor stored.
- Can be disabled at any time from the Settings screen.

---

## 6. Camera and Image Access

- **QR Scanning:** The camera is used solely to read QR codes. No footage is recorded or stored.
- **OCR Scanning:** The image you select is temporarily processed for URL detection and is automatically deleted from our servers after analysis is complete.

---

## 7. Data Retention

| Data | Retention Period |
|------|-----------------|
| Query history | Until you delete it or request account deletion |
| Technical metrics | 90 days |
| Crash reports (Sentry) | 90 days |
| Anonymous usage statistics | Indefinite (cannot be linked to an individual) |
| OCR images | Deleted immediately after analysis |

---

## 8. Data Security

- All communications are protected by HTTPS/TLS encryption.
- API keys and sensitive information are stored only server-side and are never exposed within the application.
- Database access is restricted through Row Level Security (RLS) policies.
- Your query records are only accessible via your device identifier.

---

## 9. Your Rights and Data Deletion

**You have the right to delete your data.**

You can delete all your data from within the app:
1. Open the Profile screen
2. Go to the Settings tab
3. Tap "Delete All My Data"
4. After confirmation, the following data is permanently deleted:
   - All query history
   - Usage statistics
   - Device registration

**Note:** Anonymous technical metrics (response times, usage events) may be retained as they cannot be linked to an individual. These are analyzed only as aggregate statistics.

For requests under applicable data protection laws, contact us at support@sqrseal.com.

---

## 10. Children's Privacy

SQRSeal is not directed at children under the age of 13 and does not knowingly collect data from this age group. If you are a parent or legal guardian and believe your child has shared data, please contact us.

---

## 11. GDPR Compliance

If you are located in the European Economic Area (EEA), you have the following rights under the General Data Protection Regulation (GDPR):

- **Right of access:** Request a copy of your personal data.
- **Right to rectification:** Request correction of inaccurate data.
- **Right to erasure:** Request deletion of your personal data.
- **Right to restriction:** Request restriction of processing.
- **Right to data portability:** Request transfer of your data.
- **Right to object:** Object to processing of your personal data.

To exercise these rights, contact us at support@sqrseal.com.

**Legal basis for processing:**
- Legitimate interest (security analysis, app functionality)
- Consent (clipboard monitoring, which can be disabled at any time)

---

## 12. Policy Changes

We reserve the right to update this policy. For significant changes, an in-app notification will be provided. The current policy is always available at sqrseal.com/privacy.

---

## 13. Contact

For questions about our privacy policy:

**Email:** support@sqrseal.com  
**Website:** https://sqrseal.com  
**In-app:** Profile → Settings → Privacy Policy

---

*SQRSeal — Stay safe in the digital world.*
