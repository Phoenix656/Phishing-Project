# Phishing-Project
This is a project made to simulate phishing attacks in a controlled environment to assess and improve user awareness and response to social engineering threats. The project aims to identify human vulnerabilities in cybersecurity and promote safe online behavior through real-world phishing scenarios

# Phishing Simulation Lab (GoPhish).

This lab demonstrates how a phishing campaign is orchestrated from the attacker's perspective using GoPhish. The goal was to build a full end-to-end simulation—from template design to credential capture—within a localized, ethical framework.

# 🛠 Setup & Tech Stack

1) Framework: GoPhish (v0.12.1)
2) Email Capture: MailHog (Used as a local SMTP relay to prevent real emails from leaving the lab)
3) Environment: Localhost / Virtualized Network
4) Frontend: HTML5/CSS3 for landing page clones

# 🧪 Simulation Workflow
1. The Hook (Template Design)
   
      ➡️I designed an email template focused on urgency-based social engineering. The "Password Expiring" hook was used to trigger a fast response from the user.
   
      ➡️Dynamic Links: Used {{.URL}} to track specific user IDs.
   
      ➡️Tracker: Embedded the GoPhish tracking pixel to monitor "Email Opens."

3. The Capture (Landing Page)
   
      ➡️Created a "Security Verification" page. When a user submits the form:
   
      ➡️GoPhish captures the POST request.
   
      ➡️Ethics Check: The simulation was configured to "Capture Credentials" but not store them in plain text, demonstrating the vulnerability without compromising data.

3. Redirection
   
      ➡️Upon clicking "Submit," users were redirected to the actual legitimate login page of the service being simulated. This is a common tactic to make the victim think the login was simply a "timeout" or     "refresh" error.

# ⚠️ Key Learnings & Troubleshooting
  SMTP Handshakes: Initially, delivery failed because the GoPhish sending profile didn't match the MailHog port. Fixed by adjusting the SMTP settings to localhost:1025.

  Template Rendering: Learned that many email clients strip modern CSS. Had to revert to inline styles and tables for the template to look professional.

  Psychology: Urgency is a massive driver. 60% of clicks happened within the first 5 minutes of the "expiring" notification.

# 📁 Repository Structure
    /templates - The HTML source for the "Security Alert" emails.

    /landing-pages - Mock login page code.

    /logs - Exported CSV data from the GoPhish dashboard (redacted).

# ⚖️ Ethics & Legal
This project is for educational purposes only.

No real brands were impersonated.

No data was sent over the public internet.

Targeted users were aware they were part of a security test group.

# Author
Krrish Maheshwari / Phoenix.

CyberSecurity Intern.

