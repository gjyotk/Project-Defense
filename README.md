# Project-Defense


## Introduction

Project Defense focuses on the real-time surveillance and analysis of network activity across multiple devices. The project utilizes advanced Machine Learning algorithms and Generative AI to enhance Cybersecurity by analyzing time-series data from network logs. Machine Learning is used for anomaly detection and predictive analysis to identify unusual patterns that signal potential cyber attacks.

The system is designed to automatically respond to threats in real-time using a combination of Python scripts and Bash automation. Python scripts are employed to detect specific attack indicators and anomalies based on predefined conditions. Upon identification of an attack marker, these scripts initiate predefined actions, such as blocking malicious IP addresses or sending alerts, to proactively manage and neutralize threats. This integrated approach enhances the system's capability to protect against cyber attacks effectively and efficiently.



## Objectives

- Regularly Review Logs: Periodically review and monitor logs from IDS, firewalls, and other network devices.

- Set Alerts: Configure alerts for malicious and fraudulent activities.

- Baseline Normal Behavior: Establish a baseline for normal network activity to more easily identify anomalies.

- Use Threat Intelligence: Integrate threat intelligence feeds to stay updated on known malicious IPs and domains.

- Fraud Prediction and Prevention: Using advanced ML algorithms, Python Scripts and Generative  AI to predict and Bash Scripting to prevent potential cyber frauds.



## System Design


<img src="https://github.com/user-attachments/assets/c2fc6335-e1b5-4487-9eb8-2dbf08e21369" alt="drawing" width="460"/>


## Setup instructions

- install VM-ware workstation
- install Mininet
- install Elasticsearch
- Setup a syslog server 



## Implemented System



## Description of the Implemented system



### Data collection



### Detection

The anomaly detection module will receive the collected network data and employ advanced machine learning (ML) techniques to conduct flow-based detection. This process involves analyzing network flows to classify each one as either normal or abnormal. The machine learning algorithms will be trained to recognize patterns and anomalies within the data, ensuring accurate and efficient detection of threat.

When an aberrant flow is identified, it will be flagged and sent to the prevention module. This module is responsible for taking immediate action to neutralize the threat. Actions may include blocking the source IP address, terminating the malicious connection, or alerting the network administrators via an SMS. The goal is to stop the source of the attack promptly, minimizing potential damage and maintaining network integrity. Twilio is used to send alert to the network administrator when a threat is detected.

If a flow is classified as normal, no further action will be taken, allowing regular network activity to continue uninterrupted. This automated approach ensures that only suspicious activities trigger a response, thereby reducing false positives and maintaining optimal network performance.


### Prevention

<img width="332" alt="Screenshot 2024-07-24 at 2 38 51 AM" src="https://github.com/user-attachments/assets/5c9f46ae-9541-4c63-8e84-5ee0a01f3ad7">

- INetwork Access Control (NAC) Using FreeRADIUS and pfSense:
- FreeRADIUS: For Configuring authentication and authorization of network devices and users.
pfSense: Integrated with FreeRADIUS for network access control, enforcing policies, and managing access.
- Regular Software Updates: Keeping all systems, applications, and devices up-to-date with the latest patches and security updates to protect against known vulnerabilities.
- Network Segmentation: Dividing the network into segments to limit the spread of malware and restrict access to sensitive data and systems.
- Intrusion Detection and Prevention Systems (IDPS): Deployed IDPS to monitor network traffic for suspicious activities and automatic response to potential threats.
- Firewalls and Access Control Lists (ACLs): Using firewalls and ACLs to control incoming and outgoing network traffic based on predefined security rules.




## Results & Discussion


- Random forest Classifier-
  1. Accuracy_score: 100.0
  2. precision_score: 100.0
  3. recall_score: 100.0
  4. f1_score: 100.0

- Logistic Regression
  1. Accuracy_score: 98.4375
  2. precision_score: 100.0
  3. recall_score: 90.0
  4. f1_score: 94.73684210526316
     
- Decision Tree
  1. Accuracy_score: 100.0
  2. precision_score: 100.0
  3. recall_score: 100.0
  4. f1_score: 100.0
 
- Naive Bytes
  1. Accuracy_score: 93.75
  2. precision_score: 71.42857142857143
  3. recall_score: 100.0
  4. f1_score: 83.33333333333333
- KNN
  1. Accuracy_score: 98.4375
  2. precision_score: 100.0
  3. recall_score: 90.0
  4. f1_score: 94.73684210526316
 
  
## Conclusion
The project successfully establishes a comprehensive framework for network security, integrating advanced monitoring, automated incident response, and robust access control mechanisms. Through our multifaceted approach, this project not only enhances the ability to detect and mitigate threats in real-time but also lays a solid foundation for ongoing network security management. This integrated system ensures that the network remains secure, resilient, and capable of adapting to evolving threats, thereby safeguarding organizational assets and maintaining operational integrity.



















