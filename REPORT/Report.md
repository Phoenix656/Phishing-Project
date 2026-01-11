Phishing Awareness Simulation Report

Using GoPhish

1. Introduction

Phishing is one of the most common and effective cyber-attacks, primarily because it exploits human behavior rather than technical vulnerabilities. Attackers often rely on urgency, fear, and authority to manipulate users into clicking malicious links or revealing sensitive information.

This project presents a phishing awareness simulation conducted using the GoPhish framework. The objective was to demonstrate how phishing campaigns are structured, how users interact with them, and why awareness training is critical for cybersecurity defense.

The project was executed strictly in a controlled local environment for educational purposes.

2. Objectives

The primary objectives of this project were:

To simulate a real-world phishing scenario in a safe environment

To understand how users respond to urgency-based phishing emails

To demonstrate phishing URL generation and interaction tracking

To highlight the importance of cybersecurity awareness

To follow ethical and responsible security testing practices

3. Tools and Technologies Used

GoPhish – Open-source phishing simulation framework

HTML/CSS – For creating a realistic landing page

Localhost Environment – For controlled testing

Web Browser – For interaction simulation and validation

4. Methodology
4.1 Campaign Setup

GoPhish admin server configured on https://127.0.0.1:3333

Phishing server configured on http://127.0.0.1:8080

A phishing email template was created using urgency-based messaging

A login-style landing page was designed to simulate credential entry

4.2 Email Template

The email used a password expiry alert theme, which is a commonly observed phishing tactic.
The message included:

A security warning

A 24-hour deadline

A dynamically generated phishing URL ({{.URL}})

4.3 Landing Page

The landing page mimicked a basic account verification form

Credential storage was disabled

Submissions were used only to record interaction events

Users were redirected after interaction to safely terminate the phishing flow

4.4 Campaign Execution

A small group of test users was selected

The campaign was launched manually

Email delivery was simulated due to SMTP/network restrictions

User interaction was validated by accessing the generated phishing URLs

5. Results
5.1 Campaign Metrics
Metric	Count
Emails Sent	5
Emails Opened	1
Links Clicked	1
Data Submitted	0
Emails Reported	0
5.2 Observations

At least one user interacted with the phishing content

The phishing URL and landing page functioned correctly

No sensitive data was submitted

The GoPhish timeline successfully logged interaction events

6. Extended Analysis

Although the campaign size was small, the results are significant.
A single successful click is enough to validate phishing risk, as real-world attackers often require only one compromised user to initiate larger attacks.

The results reinforce the idea that phishing success depends heavily on human psychology, not technical flaws. The absence of data submission also highlights that awareness and hesitation can reduce the impact of phishing even after a link is clicked.

7. Ethical Considerations

Ethics were prioritized throughout this project:

No real credentials were collected or stored

No real organizations were targeted

Only test accounts were used

Public documentation avoids impersonating real brands

The project was conducted strictly for educational purposes

A detailed ethics statement is provided in ethics/ethical-considerations.md.

8. Limitations

Small sample size limits statistical conclusions

Email delivery was subject to local SMTP and network restrictions

Results demonstrate behavior patterns rather than large-scale risk

9. Conclusion

This phishing awareness simulation demonstrates that phishing remains a serious cybersecurity threat due to human factors. Even in a controlled environment, user interaction with phishing content was observed, highlighting the need for continuous awareness training and user education.

The project successfully validates the use of GoPhish as an effective tool for cybersecurity awareness simulations and reinforces the importance of ethical, controlled security testing.

10. Future Scope

Larger-scale phishing awareness campaigns

Pre- and post-training comparison studies

Integration with security awareness programs

Advanced phishing scenarios such as spear-phishing

11. Disclaimer

This project is intended only for educational and awareness purposes.
Any misuse of the demonstrated techniques outside a permitted environment is strictly discouraged.

Author: Phoenix
Project Type: Cybersecurity Awareness Simulation
Tool Used: GoPhish