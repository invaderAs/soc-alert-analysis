# SOC120 – Phishing Mail Detected (Internal to Internal)

Platform: LetsDefend  
Severity: Low  
Verdict: False Positive  

## Alert Summary
This alert was triggered for a suspected phishing email sent between two internal users. Since internal-to-internal emails can sometimes be flagged by detection rules, the alert was reviewed to confirm whether any real threat was present.

## Email Details
- **Sent Time:** Feb 07, 2021, 04:24 AM  
- **SMTP Address:** 172.16.20.3  
- **Sender Address:** john[@]letsdefend.io  
- **Recipient Address:** susie[@]letsdefend.io  

## Investigation
The email headers and content were reviewed as part of the investigation. The SMTP address belonged to an internal IP range, and both the sender and recipient addresses were internal users from the same domain.

The email content did not appear suspicious, and there were no URLs or attachments included in the message. No indicators commonly associated with phishing emails were identified.

## Findings
- The email was sent from an internal SMTP address  
- Both sender and recipient were internal users  
- The email content was not suspicious  
- No attachments or URLs were present  

## Conclusion
This alert was confirmed as a false positive. The email was a legitimate internal communication and did not pose any security risk.

The alert was closed after verification, and no further action was required.

## Screenshot
![SOC120 Alert Screenshot](../screenshots/soc120.png)
