# Automated-Security-Alerts-with-Python

The following is an example of how a security team might respond to and investigate suspicious network behavior using a Python security alert. 

**Scenario**: Late-Night File Access on Patient Records System at City General Hospital, a large busy hospital in a major metropolitan area. The Security Operations Center team monitors the hospital's IT systems around the clock. Sarah, the new SOC analyst is on the night shift. At 3:15 AM, the automated Python security alert system triggers the following message in the SOC console.

**The Investigation**: Sarah sees the following security alert pop up on her screen. This Python script tells us that a user named 'nurse_johnson' accessed a patient record for 'Jane Doe' at 3:15 AM. The alert came from the log files that track access to the hospital's sensitive patient records system. The keyword that triggered the alert was "accessed" which our Python script was set to look for. This is potentially suspicious because while some nurses may need to access records at this hour, it's worth investigating if Nurse Johnson should be accessing a specific patient's records in the middle of the night. Is she on duty at this hour? Does she have a legitimate reason to access this record at this specific time?







**Preliminary  Research**: Sarah will check the hospital schedule to see if Nurse Johnson is working the night shift. Additionally, she will verify through a secure interface to see if Nurse Johnson is assigned to Jane Doe's medical care team. There are 2 potential outcomes from her preliminary research.

A. Legitimate Access: If Nurse Johnson is on duty and is a member of Jane Doe's care team then we can conclude the access was likely legitimate. In this case, this could be resolved as a false positive. 

B. Suspicious Access: If Nurse Johnson is not scheduled to work that night or if she is not assigned to Jane Doe's care team, the late-night access would be highly suspicious. It is also possible that Nurse Johnson's login credentials were stolen or in a less likely scenario, a system malfunction generated a "accessed" log alert. Regardless of the reason, this should be further investigated. 

**Escalation and Further Investigation**: Based on the suspicious findings, Sarah should escalate the alert to a senior SOC analyst. Further investigation might involve checking other log files for activity from Nurse Johnson's account, analyzing network traffic associated with the access using a SIEM tool and potentially locking Nurse Johnson's account until the activity can be verified as legitimate. 

**Conclusion**: The Python script acted as an automated watchman. It was programmed to look for specific words related to activity that is being monitored and when it found one, it raised a red flag. 


Based on current trends and the capabilities of Python in security automation, here are ten common security alerts that are frequently detected and automated using Python. Code automation is critical for managing the high volume and sophistication of cybersecurity attacks and monitoring modern networks. 


1. **Multiple Failed Login Attempts**

2. **Detection of Known Malicious IPs/Domains**

3. **Anomalous Network Traffic**

4. **Unauthorized File Access**

5. **Changes to Critical System Files**

6. **Phishing Link/Keyword Detection in Emails**

7. **New and Unexpected Software Installations**

8. **Privilege Escalation Attempts**

9. **Data Exfiltration Indicators**

10. **Anomalous User Behavior**


