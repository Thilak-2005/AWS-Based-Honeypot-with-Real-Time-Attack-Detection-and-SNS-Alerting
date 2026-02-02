# AWS-Based-Honeypot-with-Real-Time-Attack-Detection-and-SNS-Alerting
This project demonstrates the implementation of an **AWS-based honeypot system** designed to attract, detect, and monitor malicious network activity in a cloud environment.  
A publicly exposed EC2 instance is intentionally configured as a decoy server to capture real-world attack traffic.  
The system uses **AWS-native monitoring and alerting services** to simulate a real SOC (Security Operations Center) workflow.

---

## Objectives
- Deploy a cloud-based honeypot using AWS
- Attract and monitor real attacker traffic
- Capture attacker IPs and network behavior
- Centralize logs for analysis
- Generate real-time security alerts using SNS

---

## 🧱 Architecture Overview

![](architecture.png)


---

## Technologies Used
- **AWS EC2** – Honeypot server
- **AWS VPC** – Network isolation
- **Security Groups** – Open ports to attract attackers
- **VPC Flow Logs** – Capture network traffic
- **AWS CloudWatch** – Log storage and monitoring
- **AWS SNS** – Email alert notifications
- **AWS IAM** – Secure role-based access
- **AWS CloudTrail** – API activity logging

---

### Honeypot EC2 Instance
![](honeypot-ec2.png)

### Security Group Configuration
![](securitygroup.png)

### VPC Configuration
![](vpc-honey.png)

### IAM Role Creation
![](Iamrolecreation.png)

### IAM Role Attached
![](IAMrole.png)

### VPC Flow Logs Creation
![](vpcflowlogscreation.png)

### VPC Flow Logs
![](VPC-flowlog.png)

### VPC Flow Traffic
![](VPC-flow.png)

### CloudWatch Logs
![](clouudwatch.png)

### CloudWatch Alarm
![](snsaleram.png)

### CloudTrail Creation
![](cloudtrailcreation.png)

### CloudTrail Logs
![](cloudtrail.png)

### Attacker Simulation
![](attacker.png)

### SNS Email Alert
![](SMSalertEmail.png)

### Logs Stored in S3
![](s3-store-logs.png)

---

- Successfully captured real attacker traffic
- Identified malicious source IP addresses
- Implemented centralized log monitoring
- Generated real-time security alerts
- Simulated SOC-level detection workflow




