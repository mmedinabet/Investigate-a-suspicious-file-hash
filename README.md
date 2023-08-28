
<h1>Investigate a suspicious file hash and respond alert</h1>
<h2>Description</h2>
In your role as a Level One analyst within the Security Operations Center (SOC) of a financial services firm, you've recently been alerted to a concerning incident. This incident involves the download of a suspicious file onto an employee's workstation.

Upon receiving the alert, you've taken on the responsibility of delving into the matter. Your investigation has unveiled that the employee in question received an email containing an attachment. The attachment took the form of a password-protected spreadsheet, with the password conveniently supplied within the same email. The employee proceeded to download this file and utilized the provided password to unlock its contents. Regrettably, upon accessing the file, a malevolent payload was activated on the employee's computer.

As part of your actions, you've successfully recovered the malicious file itself. In addition, you've generated a SHA256 hash value for this file. Drawing from your prior knowledge, which you gained through a previous course, you understand that a hash function operates as an algorithm producing an encrypted code that remains impervious to decryption. This cryptographic technique of hashing is indispensable for establishing a distinct identity for malware, akin to a one-of-a-kind digital fingerprint for each file.

<h2> Alert Description</h2>

SHA256 file hash: 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b

Here is a timeline of the events leading up to this alert:

- <b>1:11 p.m.: An employee receives an email containing a file attachment.</b>

- <b>1:13 p.m.: The employee successfully downloads and opens the file.</b>

- <b>1:15 p.m.: Multiple unauthorized executable files are created on the employee's computer.</b>

- <b>1:20 p.m.: An intrusion detection system detects the executable files and sends out an alert to the SOC.</b>

<h2>I decided to use VirusTotal to analize the malicious file</h2>
I entered the SHA256 file hash in the search box to determine that the file hash has been reported as malicious by 58 vendors and 2 sandboxes reports. 

![Screenshot 2023-08-26 9 44 36 PM](https://github.com/mmedinabet/Investigate-a-suspicious-file-hash/assets/142737434/ff4a05c1-2a75-4bef-a240-0a3851aecb58)


<h2> Pain Pyramid</h2>

![Screenshot 2023-08-26 9 46 24 PM](https://github.com/mmedinabet/Investigate-a-suspicious-file-hash/assets/142737434/cefae166-6a29-4383-8a74-0c919fbb0909)

<h2>Incident Handler's Report</h2>

![Screenshot 2023-08-26 10 06 05 PM](https://github.com/mmedinabet/Investigate-a-suspicious-file-hash/assets/142737434/f3d16663-db67-4743-a4f4-64f0bfc4b8fe)

<h2> </h2>
After investigating the email attachment file's hash, the attachment has already been verified malicious. Now that you have this information, you must follow your organization's process to complete your investigation and resolve the alert.

<h2>Use a playbook to respond to a phishing incident</h2>
Physing Flowchart is provided by the Financial Services Firm. The flowchart is part of the playbook which is considered the manual or step-by-step process to respond to certain incidents. 

![Screenshot 2023-08-28 3 05 34 PM](https://github.com/mmedinabet/Investigate-a-suspicious-file-hash/assets/142737434/c9b5240c-1018-49ae-9419-6af7d89201c2)

<h2>Completed Alert Ticket</h2>

![Screenshot 2023-08-28 3 03 24 PM](https://github.com/mmedinabet/Investigate-a-suspicious-file-hash/assets/142737434/89467da7-613c-414b-9e61-057c9c8ab180)


![Screenshot 2023-08-28 3 03 50 PM](https://github.com/mmedinabet/Investigate-a-suspicious-file-hash/assets/142737434/3a5c5ac8-372b-4799-884f-9018d0fec250)

