Phishing Email Analysis \& Incident Investigation:



Objective:



Analyze a suspicious email sample and investigate its headers, sending IP address, and embedded URL to identify potential phishing or malicious indicators.



Investigation Workflow:



Email Sample  

↓  

Email Header Analysis  

↓  

Identify Sending IP  

↓  

Virus Total IP Investigation  

↓  

Inspect Email HTML  

↓  

Extract Suspicious URL  

↓  

Virus Total URL Investigation  

↓  

Document Findings



Tools Used:



\- Google Admin Toolbox Message header

\- Virus Total



Email Analysis:



Sender: OneCasino <132784@534617.vav.proo55.us.com>



Subject: Welcome gift inside: 50 spins waiting for you



Return-Path: bounce@vav.proo55.us.com



Sending IP: 141.95.0.46



SPF: Pass



DKIM: Pass for vav.proo55.us.com



The email headers were analyzed to identify the sender infrastructure and determine the originating IP address.



IP Investigation:



The sending IP address 141.95.0.46 was investigated using Virus Total.



Some security vendors reported malicious or phishing-related classifications, while other vendors reported the IP as clean.



URL Investigation:



The email's HTML source contained the following URL:



`https://tinyurl.com/mrymsuhv`



The URL was analyzed using Virus Total without directly opening the link.



Virus Total showed \*\*3/91 security vendors\*\* with detections. The observed classifications included \*\*Phishing\*\* and \*\*Malicious\*\*.



Indicators of Compromise (IOCs):



| Indicator | Value |

| Sender Domain | vav.proo55.us.com |

| Sending IP | 141.95.0.46 |

| Suspicious URL | https://tinyurl.com/mrymsuhv |



Security Concepts Demonstrated:



\- Email Header Analysis

\- IOC Identification

\- IP Reputation Analysis

\- URL Analysis

\- Phishing Investigation

\- Security Alert Investigation

\- Evidence Collection

\- Incident Documentation



Evidence:



Email Header Analysis:



!\[Email Header Analysis](screenshots/01\_real\_email\_header\_analysis.png)



&#x20;Virus Total IP Analysis:



!\[Virus Total IP Analysis](screenshots/02\_virustotal\_ip\_analysis.png)



Virus Total URL Analysis:



!\[Virus Total URL Analysis](screenshots/03\_virustotal\_url\_analysis.png)



Investigation Conclusion:



The email was assessed as suspicious based on the email content, shortened URL, sending infrastructure, and security-vendor detections.



The collected evidence demonstrates a basic SOC workflow for analyzing a suspicious email and investigating related indicators of compromise.







