---
title: "Week 6 Worklog"
date: 2026-10-19
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### OBJECTIVES IN WEEK 6:
- Prepare for the 26 October Well-Architected review; examine the forecast protocol and baseline/challenger evidence.
- Develop familiarity with in-memory caching with Amazon ElastiCache (Redis): create clusters, connect via CLI/SDK and work with data.
- Read and review CPAWS proposal/API documentation, aligning product goals and evaluation criteria.
- Practice advanced networking: Transit Gateway, Site-to-Site VPN (with Cisco CSR), ECMP routing and Hybrid DNS with Route 53.
- Review the CPAWS architecture and baseline/challenger evidence during the 19–22 October team discussions.

### TASKS OF WEEK 6:

| Day | Task | Start Date | End Date | References |
|:---:|---|:---:|:---:|---|
| **Mon** | **- Team project meeting: identify and research the solution architecture for the web app**<br>+ Cross-checked the previously reviewed API contract against the EventBridge Scheduler → Lambda ingest → S3 → Lambda predict → DynamoDB → API Gateway → web flow to understand data availability and forecast timing<br>+ Reviewed EDA, NYSE/CME calendars, abnormal prices (especially negative WTI on 20 Apr 2020) and no-future-data requirements<br>+ Focused on the interface between cleaned prices, session-based log-return targets and evaluation metrics | 19/10/2026 | 19/10/2026 | [CPAWS repository](https://github.com/CPAWS-AWS-FCAJ/CPAWS-commodity-forecasting) |
| **Tue** | **- Practice Lab 16: Amazon ElastiCache - Redis**<br>+ Introduction<br>+ Preparation<br>* Create an AWS Access Key<br>* Install the AWS CLI<br>* Configure the AWS CLI<br>+ Create an ElastiCache cluster<br>* Create a subnet group (Console/AWS CLI)<br>* Create a cluster (cluster mode disabled) (Console/AWS CLI)<br>* Create a cluster (cluster mode enabled)<br>* Grant access to the cluster<br>* Connect to a cluster node<br>Cluster Mode Disabled<br>Cluster Mode Enabled<br>Endpoints using the AWS CLI<br>* Delete the cluster (Console/AWS CLI) | 20/10/2026 | 20/10/2026 | [Lab 16 Intro](https://000061.awsfcaj.com/vi/1-introduce/)<br>[Prereq](https://000061.awsfcaj.com/vi/2-prerequiste/)<br>[Redis Lab](https://000061.awsfcaj.com/vi/3-amazonelasticacheforredis/) |
| **Wed** | **- CPAWS (alongside the lab):** Reviewed `evaluation_kind`, `target_cutoff_date`, pinball skill and the validation/test/rolling separation against ADR-0008.<br>**- Continue Lab 16: Amazon ElastiCache - Redis**<br>+ Use the AWS SDK to write and read data on ElastiCache<br>* Create an ElastiCache cluster<br>Create a cluster (cluster mode disabled)<br>Create a cluster (cluster mode enabled)<br>Check the user group<br>* Connect to ElastiCache<br>Connect to a cluster (cluster mode disabled)<br>Connect to a cluster (cluster mode enabled)<br>* Set and Get strings<br>* Set and Get a hash with multiple items<br>* Publish (write) and subscribe (read)<br>* Write and read from a stream<br>+ Clean up resources | 21/10/2026 | 21/10/2026 | [SDK Redis](https://000061.awsfcaj.com/vi/4-sdkelasticache/)<br>[Cleanup](https://000061.awsfcaj.com/vi/5.cleanupresource/)<br>[CPAWS repository](https://github.com/CPAWS-AWS-FCAJ/CPAWS-commodity-forecasting) |
| **Thu** | **- Team project meeting: finalize the solution architecture and budget estimation for the web app**<br>+ Reviewed the architecture and preliminary budget estimate to understand the scheduled Lambda approach rather than an always-on endpoint<br>+ Ran and analyzed DLinear MVP validation 2019 against the 252-session empirical quantile baseline<br>+ Cross-checked CEEMDAN–DLinear/K3 experiments, pinball skill and reasons challengers did not consistently beat the baseline | 22/10/2026 | 22/10/2026 | [AWS Pricing Calculator](https://calculator.aws/#/)<br>[PyEMD (CEEMDAN)](https://pyemd.readthedocs.io/)<br>[CPAWS repository](https://github.com/CPAWS-AWS-FCAJ/CPAWS-commodity-forecasting) |
| **Fri** | **- Explore a new AWS topic (alongside the lab):** Read an overview of NVIDIA Isaac Lab and SageMaker HyperPod versus Training Jobs; learned about GPU jobs, containers and checkpoints without running a training job.<br>**- Practice Lab 17: AWS Networking and Content Delivery**<br>+ Introduction<br>+ Preparation<br>* Deploy the VPCs<br>* Cisco CSR Agreement<br>+ VPC Components Deep Dive<br>+ Transit Gateway and Site-to-Site VPNs<br>* Transit Gateway and Site-to-Site VPNs<br>* Access the Cisco CSR Router with Cloud9<br>* Set up the Site-to-Site VPN<br>* Add an ECMP path<br>* Transit Gateway routing<br>+ Route 53 DNS Endpoints and Internal Hosted Zones<br>* Deploy DNS<br>* Test DNS | 23/10/2026 | 23/10/2026 | [Lab 17 Intro](http://000092.awsfcaj.com/vi/1-introduce/)<br>[VPC Deep Dive](https://000092.awsfcaj.com/vi/3-vpcs/)<br>[TGW & VPN](https://000092.awsfcaj.com/vi/4-transitgatewayandvpn/)<br>[Route 53](https://000092.awsfcaj.com/vi/5-route53/)<br>[Isaac Lab documentation](https://isaac-sim.github.io/IsaacLab/)<br>[SageMaker AI documentation](https://docs.aws.amazon.com/sagemaker/) |

### ACHIEVEMENTS IN WEEK 6:

1. Completed Lab 16: learned Amazon ElastiCache (Redis), created clusters, connected and worked with advanced data features (Pub/Sub, Stream) via the AWS SDK.
2. Completed the first part of Lab 17 (continued in Week 7): deployed a complex network using Transit Gateway with VPN to a Cisco CSR router, configured ECMP routing and hybrid DNS resolution with Route 53.
3. Reviewed the serverless architecture and budget from the Modeling & Evaluation perspective; implementation was owned by the Platform contributors.
4. Reviewed EDA, quality flags, trading calendars and negative WTI prices; evaluated DLinear/K3 against the 252-session baseline on validation 2019.
5. Read about Isaac Lab, SageMaker HyperPod and Training Jobs to understand infrastructure choices for robot training.

