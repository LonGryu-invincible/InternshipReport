---
title: "Week 7 Worklog"
date: 2026-10-26
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### OBJECTIVES IN WEEK 7:
- Strengthen advanced networking skills: VPC Endpoints (PrivateLink), VPC Peering and centralized network management with Transit Gateway Network Manager.
- Practice deploying a real web application (WordPress) with a highly available architecture (ASG, ALB, RDS, CloudFront).
- Master the "Infrastructure as Code" (IaC) mindset with AWS CloudFormation to automate infrastructure provisioning.
- Participate in the 26 October AWS HCM volunteering activity and review CPAWS S1a shadow and API/evaluation semantics.

### TASKS OF WEEK 7:

| Day | Task | Start Date | End Date | References |
|:---:|---|:---:|:---:|---|
| **Mon** | **- Joined the AWS HCM STEM stuffed-animal volunteer event**<br>**- Team meeting: assess Well-Architected criteria and revise the project architecture**<br>+ Discussed Lambda container batch inference, cost and reproducibility<br>+ Reviewed h=1–7 session log-return targets, seven quantiles, endpoint validity and pinball skill against `baseline-q252`<br>+ Summarized DLinear/K3 findings and champion-versus-challenger criteria | 26/10/2026 | 26/10/2026 | [AWS Well-Architected](https://aws.amazon.com/architecture/well-architected/)<br>[Proper Scoring Rules](https://doi.org/10.1198/016214506000001437) |
| **Tue** | **- Continue Lab 17:**<br>+ VPC Endpoints for AWS services<br>* Deploy a VPC Endpoint<br>* Test the VPC Endpoint<br>+ VPC Endpoint Services<br>* Deploy VPC Endpoint Services<br>+ VPC Peering<br>* VPC Peering Request<br>* Routing configuration<br>* Test VPC Peering<br>+ Transit Gateway Network Manager<br>* Set up Network Manager<br>* Configure Sites<br>* Network Insights<br>+ Clean up resources | 27/10/2026 | 27/10/2026 | [VPC Endpoint](https://000092.awsfcaj.com/vi/6-vpcendpointaws/)<br>[PrivateLink](https://000092.awsfcaj.com/vi/7-vpcendpointonpremise/)<br>[Peering](https://000092.awsfcaj.com/vi/8-vpcpeering/)<br>[Network Manager](https://000092.awsfcaj.com/vi/9-transitgatewaynetworkmanager/) |
| **Wed** | **- CPAWS (alongside the lab):** Reviewed the S1a (`s1a-l094`) shadow proposal, volatility scaling and its separation from the champion.<br>**- Practice Lab 18: Deploy WordPress on AWS Cloud**<br>+ Introduction<br>+ Preparation<br>* Prepare the VPC and Subnets<br>* Create a Security Group for EC2<br>* Create a Security Group for the Database Instance<br>* Launch an EC2 Instance<br>* Launch a Database Instance<br>+ Install WordPress on EC2<br>+ Set up Auto Scaling for the WordPress instance<br>* Create an AMI from the web server instance<br>* Create a Launch Template<br>* Create a Target Group<br>* Create a Load Balancer<br>* Create an Auto Scaling Group<br>+ Database backup and restore<br>* Create a DB snapshot<br>* Restore from the DB snapshot<br>+ Create CloudFront for the web server<br>+ Clean up resources | 28/10/2026 | 28/10/2026 | [SDK Redis](https://000061.awsfcaj.com/vi/4-sdkelasticache/)<br>[Cleanup](https://000061.awsfcaj.com/vi/5.cleanupresource/)<br>[Lab 18 Intro](https://000101.awsfcaj.com/vi/1-introduce/)<br>[Install WP](https://000101.awsfcaj.com/vi/3-installwordpressonec2/)<br>[ASG Setup](https://000101.awsfcaj.com/vi/4-asgforec2/)<br>[CloudFront](https://000101.awsfcaj.com/vi/6-createcloudfront/) |
| **Thu** | **- Finalize the CPAWS proposal**<br>+ Cross-checked proposal requirements with API quantiles, `normalize_quantiles()` and `prob_up` rules<br>+ Reviewed metrics, trading calendars, provenance and walk-forward evaluation rather than claiming ownership of API implementation<br>+ Summarized S1a volatility-scaling experiments; kept `baseline-q252` champion and S1a as a shadow challenger | 29/10/2026 | 29/10/2026 | [API Gateway REST API](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-rest-api.html) |
| **Fri** | **- Explore a new AWS topic (alongside the lab):** Read the AWS Physical AI Toolchain introduction and noted the cycle of real-world data → simulation → training → validation → edge deployment.<br>**- Practice Lab 19: AWS CloudFormation**<br>+ Introduction<br>+ Preparation<br>* Create an IAM User<br>* Create an IAM Role<br>+ CloudFormation basics<br>* Create a workspace<br>* Create a CloudFormation Template<br>+ Advanced CloudFormation<br>* Custom resources<br>Create a Lambda function<br>Create a stack<br>Connect to the EC2 Instance<br>* Mappings and StackSets<br>* Drift Detection<br>+ Clean up resources | 30/10/2026 | 30/10/2026 | [Lab 17 Intro](http://000092.awsfcaj.com/vi/1-introduce/)<br>[VPC Deep Dive](https://000092.awsfcaj.com/vi/3-vpcs/)<br>[TGW & VPN](https://000092.awsfcaj.com/vi/4-transitgatewayandvpn/)<br>[Route53](https://000092.awsfcaj.com/vi/5-route53/)<br>[Lab 19 Intro](https://000037.awsfcaj.com/vi/1-introduce/)<br>[CF Basic](https://000037.awsfcaj.com/vi/3-cloudformationbasic/)<br>[CF Advanced](https://000037.awsfcaj.com/vi/4-cloudformationadvance/) |

### ACHIEVEMENTS IN WEEK 7:

1. Deployed secure network connectivity: VPC Endpoints (private access to AWS services) and VPC Peering (between VPCs).
2. Built a complete WordPress system with Auto Scaling, load balancing (ALB) and global content delivery (CloudFront).
3. Mastered RDS backup & restore with snapshots in a real scenario.
4. Became proficient with AWS CloudFormation: writing templates (Infrastructure as Code), managing stacks and detecting configuration drift.
5. Reviewed the CPAWS architecture and forecast protocol: session-based targets, seven quantiles, pinball skill and leakage safeguards.
6. Reviewed the proposal, API contract and evaluation ADRs; summarized DLinear/K3/K3b/S1a experiments, retained `baseline-q252` as champion and prepared S1a for shadow evaluation.
7. Contributed to the charity activity making STEM stuffed animals for children with the AWS HCM team.
8. Began exploring Physical AI Toolchain and the connection among simulation, training and robot deployment.

