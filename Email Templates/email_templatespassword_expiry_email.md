# Phishing Email Template – Password Expiry Notification

## Overview
This email template was used as part of a **controlled phishing awareness simulation**
conducted using the GoPhish framework. The template demonstrates how attackers use
urgency and authority to manipulate users into clicking malicious links.

---

## Template Configuration (As Used)

**Template Name:** New_1  
**Email Type:** Plain Text  
**Subject:** Security Alert: Password Expiry Notification  

**Envelope Sender (Simulation Only):**
googlepley-noreply@google.com

yaml
Copy code

> Note: This sender address was used strictly within a **local testing environment**
> for educational purposes. No real emails were delivered to external users, and no
> real organization was targeted.

---

## Email Body

Dear User,

We detected unusual activity on your account.
For security reasons, your password will expire within 24 hours.

Please verify your account immediately using the link below:

{{.URL}}

Failure to act may result in temporary account suspension.

yaml
Copy code

---

## Technical Notes
- `{{.URL}}` is a GoPhish dynamic placeholder.
- During campaign execution, GoPhish automatically replaces this placeholder
  with a **unique tracking URL** for each recipient.
- This allows tracking of link clicks and landing page interactions.

---

## Psychological Techniques Demonstrated
- **Urgency:** 24-hour deadline
- **Fear:** Threat of account suspension
- **Authority:** Security alert messaging

These techniques are commonly observed in real-world phishing attacks.

---

## Ethical Disclaimer
- This template was used only in a **controlled local environment**
- No real credentials were collected
- No real Google services were accessed
- The purpose was **security awareness and education**, not exploitation