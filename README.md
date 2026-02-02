# AWS-Based-Honeypot-with-Real-Time-Attack-Detection-and-SNS-Alerting
## 📌 Project Overview
This project demonstrates the implementation of an **AWS-based honeypot system** designed to attract, detect, and monitor malicious network activity in a cloud environment.  
A publicly exposed EC2 instance is intentionally configured as a decoy server to capture real-world attack traffic.  
The system uses **AWS-native monitoring and alerting services** to simulate a real SOC (Security Operations Center) workflow.

---

## 🎯 Objectives
- Deploy a cloud-based honeypot using AWS
- Attract and monitor real attacker traffic
- Capture attacker IPs and network behavior
- Centralize logs for analysis
- Generate real-time security alerts using SNS

---

## 🧱 Architecture Overview



---

## 🛠️ Technologies Used
- **AWS EC2** – Honeypot server
- **AWS VPC** – Network isolation
- **Security Groups** – Open ports to attract attackers
- **VPC Flow Logs** – Capture network traffic
- **AWS CloudWatch** – Log storage and monitoring
- **AWS SNS** – Email alert notifications
- **AWS IAM** – Secure role-based access
- **AWS CloudTrail** – API activity logging

---

## ⚙️ Implementation Steps (High Level)

1. Created a public EC2 instance (Ubuntu) as a honeypot
2. Configured Security Groups with open SSH access
3. Enabled VPC Flow Logs for traffic monitoring
4. Stored logs in CloudWatch Log Groups
5. Created CloudWatch Alarms for abnormal traffic
6. Integrated SNS for real-time email alerts
7. Tested alerts using simulated SSH attack attempts

---

## 🚨 Alerting Mechanism
- CloudWatch monitors **NetworkIn** metrics
- When traffic crosses a defined threshold:
  - Alarm state changes to **ALARM**
  - SNS sends an **email notification**
- This simulates real-time incident detection used in SOC environments

---

## 📸 Screenshots

> Screenshots are included to demonstrate real deployment and monitoring.

### 📷 EC2 Honeypot Instance
![EC2 Instance](screenshots/ec2-instance.png)

### 📷 Security Group Configuration
![Security Group](screenshots/security-group.png)

### 📷 VPC Flow Logs
![VPC Flow Logs](screenshots/vpc-flow-logs.png)

### 📷 CloudWatch Log Group
![CloudWatch Logs](screenshots/cloudwatch-logs.png)

### 📷 CloudWatch Alarm
![CloudWatch Alarm](screenshots/cloudwatch-alarm.png)

### 📷 SNS Email Alert
![SNS Alert](screenshots/sns-alert.png)

---

## 📊 Key Outcomes
- Successfully captured real attacker traffic
- Identified source IP addresses and connection attempts
- Implemented centralized monitoring and alerting
- Gained hands-on experience with AWS cloud security services
- Simulated SOC-level detection and alert workflow

---

## 🎤 Interview Explanation (One Line)
> “I deployed an AWS-based honeypot using EC2 and monitored real attacker traffic with VPC Flow Logs, CloudWatch, and SNS-based real-time alerts.”

---

## 🚀 Future Enhancements
- Integrate SIEM (Elastic Stack / Splunk)
- Add GeoIP-based attacker visualization
- Automate IP blocking using AWS Lambda
- Map attacks to MITRE ATT&CK framework

---

## 👨‍💻 Author
**Thilak**  
Cybersecurity & Cloud Security Enthusiast  


