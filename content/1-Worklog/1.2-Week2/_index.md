---
title: "Week 2 Worklog"
date: 2026-09-21
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### OBJECTIVES IN WEEK 2:
- Master VPN troubleshooting and extend Site-to-Site connectivity with Transit Gateway.
- Understand and implement Hybrid DNS with Route 53 Resolver to resolve domain names between on-premises and AWS.
- Master multi-VPC connectivity models (VPC Peering and Transit Gateway).
- Consolidate in-depth knowledge of Compute services (EC2, AMI, EBS, Auto Scaling).
- Consolidate Compute fundamentals and participate in the early CPAWS topic exploration during the week.

### TASKS OF WEEK 2:

| Day | Task | Start Date | End Date | References |
|:---:|---|:---:|:---:|---|
| **Mon** | **- Continue Lab 5:**<br>+ Set up AWS Site-to-Site VPN:<br>5.2 Configure the VPN connection:<br>5.2.7 VPN troubleshooting guide<br>5.2.8 Official VPN troubleshooting guide from AWS<br>5.3 Configure VPN with strongSwan and Transit Gateway:<br>5.3.1 Create a Customer Gateway<br>5.3.2 Create a Transit Gateway<br>5.3.3 Create the VPN connection<br>5.3.4 Create a Transit Gateway Attachment<br>5.3.5 Configure Route Tables<br>5.3.6 Configure the Customer Gateway<br>+ Clean up resources<br>+ Infrastructure as Code Templates | 21/09/2026 | 21/09/2026 | [Lab 5 VPN](https://000003.awsfcaj.com/vi/5-vpnsitetosite/) |
| **Tue** | - Went to the office for the first time and talked with the mentor.<br>- Met, got to know and formed a team with other members of the FCAJ program. | 22/09/2026 | 22/09/2026 | [Lab 5 Prerequisite](https://000003.awsfcaj.com/vi/3-prerequisite/)<br>[Lab 5 Create EC2](https://000003.awsfcaj.com/vi/4-createec2server/) |
| **Wed** | **- Practice Lab 6: Set up Hybrid DNS with Route 53 Resolver**<br>+ Preparation:<br>* Create a Key Pair<br>* Launch the CloudFormation Template<br>* Configure Security Groups<br>+ Connect to the RDGW<br>+ Deploy Microsoft AD<br>+ Set up DNS:<br>* Create a Route 53 Outbound Endpoint<br>* Create Route 53 Resolver Rules<br>* Create Route 53 Inbound Endpoints<br>* Test the results<br>+ Clean up resources | 23/09/2026 | 23/09/2026 | [Lab 6 Prereq](https://000010.awsfcaj.com/vi/2-prerequiste/)<br>[Connect RDGW](https://000010.awsfcaj.com/vi/3-connecttordgw/)<br>[Setup AD](https://000010.awsfcaj.com/vi/4-setupad/)<br>[Hybrid DNS](https://000010.awsfcaj.com/vi/5-setuphyriddns/) |
| **Thu** | **- Practice Lab 7: Set up VPC Peering**<br>+ Preparation:<br>* Launch the CloudFormation Template<br>* Create a Security Group<br>* Create EC2 instances<br>+ Update the Network ACL<br>+ Create the Peering connection<br>+ Enable Cross-Peer DNS<br>+ Clean up resources<br>**- Practice Lab 8: AWS Transit Gateway overview**<br>+ Preparation:<br>* Create a Key Pair<br>* Launch the CloudFormation Template<br>+ Create a Transit Gateway<br>+ Create Transit Gateway Attachments<br>+ Create Transit Gateway Route Tables<br>+ Add Transit Gateway routes to the VPC Route Tables<br>+ Clean up resources | 24/09/2026 | 24/09/2026 | [Lab 7 Guide](https://000019.awsfcaj.com/vi/)<br>[Lab 8 Guide](https://000020.awsfcaj.com/vi/) |
| **Fri** | **- Team project meeting: brainstorm, analyze and research to shortlist suitable ideas**<br>+ Compared candidate ideas with regard to data availability and feasibility within the AWS project scope<br>+ Discussed forecasting gold, silver and oil; identified research questions around price sources, model evaluation and infrastructure cost<br>**- Study Module 03: Compute VM on AWS:**<br>+ 03-01: Compute VM on AWS<br>+ 03-01-01: Instance type<br>+ 03-01-02: AMI / Backup / Key Pair<br>+ 03-01-03: Elastic Block Store<br>+ 03-01-04: Instance store<br>+ 03-01-05: User data<br>+ 03-01-06: Metadata<br>+ 03-01-07: EC2 Auto Scaling<br>+ 03-02: EFS/FSx - Lightsail - MGN | 25/09/2026 | 25/09/2026 | [World Bank Commodity Markets](https://www.worldbank.org/en/research/commodity-markets)<br>[03-01](https://www.youtube.com/watch?v=-t5h4N6vfBs)<br>[03-01-01](https://www.youtube.com/watch?v=e7XeKdOVq40)<br>[03-01-02](https://www.youtube.com/watch?v=yAR6QRT3N1k)<br>[03-01-03](https://www.youtube.com/watch?v=hKr_TfGP7NY)<br>[03-01-04](https://www.youtube.com/watch?v=6IHNDJ85aoQ)<br>[03-01-05](https://www.youtube.com/watch?v=_v_43Wi7zjo)<br>[03-01-06](https://www.youtube.com/watch?v=Ew3QRaKJQSA)<br>[03-01-07](https://www.youtube.com/watch?v=bbLcPitXJSY)<br>[03-02](https://youtu.be/hFVYG8WqfU0?si=pwMJL01CuoVoxMQS) |

### ACHIEVEMENTS IN WEEK 2:

1. Completed advanced Lab 5: learned VPN troubleshooting and configured VPN with Transit Gateway (strongSwan).
2. Successfully deployed a Hybrid DNS architecture (Lab 6), configuring Inbound/Outbound Endpoints for two-way name resolution (AWS <-> on-prem).
3. Built and connected VPC networks with VPC Peering (Lab 7) and AWS Transit Gateway (Lab 8).
4. Mastered Module 03 on Compute: EC2 instance types, EBS volume types and Auto Scaling for performance and cost optimization.
5. Went to the AWS office for the first time and formed a team.
6. Joined the CPAWS team and explored candidate forecasting topics, focusing on data availability and evaluation requirements.

