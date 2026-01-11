# Campaign Configuration – Phishing Awareness Simulation

## Campaign Overview
This phishing awareness campaign was executed using the **GoPhish** framework in a
controlled local environment. The objective was to simulate a realistic phishing
scenario and observe user interaction with phishing emails and links.

---

## Campaign Details

- **Campaign Name:** Phishing Project
- **Campaign Type:** Phishing Awareness Simulation
- **Tool Used:** GoPhish
- **Environment:** Localhost (Controlled Testing)
- **Phishing Server:** http://127.0.0.1:8080
- **Admin Server:** https://127.0.0.1:3333

---

## Target Group Configuration

- **Group Name:** Test Users
- **Number of Targets:** 5
- **Target Type:** Test email accounts (Gmail and Outlook)
- **Purpose:** Controlled testing and interaction validation

No real organizational users were targeted.

---

## Email Template Used

- **Template Name:** New_1
- **Subject:** Security Alert: Password Expiry Notification
- **Email Format:** Plain Text
- **Phishing Indicator:** Dynamic URL placeholder (`{{.URL}}`)

The email content leveraged urgency and authority-based messaging to simulate
real-world phishing techniques.

---

## Landing Page Configuration

- **Landing Page Name:** Password Verification Page
- **Type:** Login-style HTML page
- **Data Capture:** Enabled (for interaction tracking only)
- **Credential Storage:** Disabled (no real credentials stored)
- **Post-Submission Redirect:** User redirected away from phishing page to safely
  terminate the simulation flow

---

## Campaign Execution

- **Launch Mode:** Manual
- **Email Delivery:** Simulated due to SMTP and network restrictions
- **Tracking Enabled:**
  - Email Sent
  - Email Opened
  - Link Clicked
  - Form Submission

The campaign was successfully launched and monitored through the GoPhish dashboard.

---

## Observed Results (Current State)

- **Emails Sent:** 5
- **Emails Opened:** 1
- **Links Clicked:** 1
- **Data Submitted:** 0
- **Emails Reported:** 0

The results demonstrate that even within a small test group, phishing emails can
successfully prompt user interaction when urgency-based messaging is used.

---

## Key Observations

- Users are more likely to interact with messages that imply immediate action.
- A single click is sufficient to demonstrate phishing susceptibility.
- Awareness simulations are effective even at a small scale.

---

## Notes
- This campaign was conducted strictly for **educational purposes**.
- No real credentials were collected or stored.
- All activity occurred in a controlled, local testing environment.
