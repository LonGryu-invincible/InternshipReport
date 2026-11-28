---
title: "Week 1 Worklog"
date: 2026-09-14
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### OBJECTIVES IN WEEK 1:
- Understand and practice secure user access management with AWS IAM.
- Master the Amazon VPC network architecture and network security layers (Security Groups, NACL).
- Implement Hybrid Cloud connectivity through AWS Site-to-Site VPN.
- Consolidate AWS networking skills through the IAM/VPC labs and VPN troubleshooting.

### TASKS OF WEEK 1:

| Day | Task | Start Date | End Date | References |
|:---:|---|:---:|:---:|---|
| **Mon** | **- Practice Lab 4: Access management with AWS Identity and Access Management (IAM)**<br>+ IAM User and IAM Group<br>+ IAM Role<br>+ Switching roles<br>**- Practice Lab 5: Getting started with Amazon Virtual Private Cloud (VPC) and AWS Site-to-Site VPN**<br>+ Introduction to Amazon VPC:<br>* Subnets<br>* Route Table<br>* Internet Gateway<br>* NAT Gateway<br>+ Network security with Security Groups and Network ACLs:<br>* Security groups<br>* Network ACLs<br>* VPC Resource Map | 14/09/2026 | 14/09/2026 | [Lab 4 Guide](https://000002.awsfcaj.com/vi/)<br>[Lab 5 Intro](https://000003.awsfcaj.com/vi/1-introduce/)<br>[Lab 5 Firewall](https://000003.awsfcaj.com/vi/2-firewallinvpc/) |
| **Tue** | **- Continue Lab 5:**<br>+ Prepare the environment:<br>* Create a VPC<br>* Create a Subnet<br>* Create an Internet Gateway<br>* Create a Route Table<br>* Create a Security Group<br>* Enable VPC Flow Logs<br>+ Deploy Amazon EC2 Instances<br>* Create EC2 Instances<br>* Test connection methods<br>* Create a Multi-AZ NAT Gateway<br>* Use Reachability Analyzer<br>* Configure an EIC Endpoint<br>* AWS Systems Manager Session Manager<br>* CloudWatch Monitoring & Alerting | 15/09/2026 | 15/09/2026 | [Lab 5 Prerequisite](https://000003.awsfcaj.com/vi/3-prerequisite/)<br>[Lab 5 Create EC2](https://000003.awsfcaj.com/vi/4-createec2server/) |
| **Wed** | **- Continue Lab 5:**<br>+ Set up AWS Site-to-Site VPN:<br>* Create the VPN environment<br>Create a VPC for the VPN<br>Create an EC2 Instance<br>* Configure the VPN connection<br>Create a Virtual Private Gateway<br>Create a Customer Gateway<br>Create the VPN connection<br>Configure the Customer Gateway<br>Customize the AWS VPN Tunnel<br>Advanced VPN configuration | 16/09/2026 | 16/09/2026 | [Lab 5 VPN](https://000003.awsfcaj.com/vi/5-vpnsitetosite/) |
| **Thu** | **- Consolidate notes from Lab 4 and Lab 5**<br>+ Redraw the VPC diagram (Subnet, Route Table, IGW, NAT Gateway) and the Site-to-Site VPN flow on draw.io<br>+ Review the differences between Security Groups and Network ACLs | 17/09/2026 | 17/09/2026 | [Lab 5 VPN](https://000003.awsfcaj.com/vi/5-vpnsitetosite/) |
| **Fri** | - Consolidate Lab 5: verify VPC route tables, security groups and VPN connectivity; review the network diagram and troubleshooting notes. | 18/09/2026 | 18/09/2026 | [Lab 5 VPN](https://000003.awsfcaj.com/vi/5-vpnsitetosite/) |

### ACHIEVEMENTS IN WEEK 1:

1. Completed Lab 4 and became proficient at creating IAM Users, Groups and Roles for proper access control.
2. Successfully built a VPC network with all components: Subnet, Route Table, IGW, NAT Gateway.
3. Configured multi-layer network security using Security Groups and Network ACLs.
4. Deployed and monitored EC2 Instances, configured secure access via Session Manager and EIC Endpoint.
5. Successfully set up an AWS Site-to-Site VPN connection between AWS and a simulated on-premises environment.

