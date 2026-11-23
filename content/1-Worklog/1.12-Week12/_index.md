---
title: "Week 12 Worklog"
date: 2026-11-23
weight: 12
chapter: false
pre: " <b> 1.12 </b> "
---

### OBJECTIVES IN WEEK 12:
- Coordinate verification of production status and Rolling Accuracy while documenting evaluation limitations.
- Review the cost figures assembled by Platform/Security and summarize Modeling & Evaluation lessons.
- Master cost and compliance governance through advanced IAM policies (limit by Region, Instance Type).
- Set up end-to-end monitoring: from the network layer (VPC Flow Logs) and the application layer (Grafana) to the AWS service layer (CloudWatch).

### TASKS OF WEEK 12:

| Day | Task | Start Date | End Date | References |
|:---:|---|:---:|:---:|---|
| **Mon** | **- Practice Lab 30: Cost and resource usage governance with IAM on AWS**<br>+ Preparation<br>* Create an IAM Group<br>* Create an IAM user<br>+ Limit by Region<br>* Create the restriction policy<br>* Attach the policy to the group<br>* Test the policy<br>+ Limit by EC2 family<br>* Create the restriction policy<br>* Attach the policy to the group<br>* Test the policy<br>+ Limit by instance size<br>* Update the restriction policy<br>* Test the policy<br>+ Limit by EBS volume<br>* Create the restriction policy<br>* Attach the policy to the group<br>* Test the policy<br>+ Clean up resources | 23/11/2026 | 23/11/2026 | [Lab 30 Intro](https://000064.awsfcaj.com/vi/1-preparation/)<br>[Limit Region](https://000064.awsfcaj.com/vi/2-limit-region/)<br>[Limit Family](https://000064.awsfcaj.com/vi/3-limit-family/)<br>[Limit Size](https://000064.awsfcaj.com/vi/4-limit-size/) |
| **Tue** | **- Practice Lab 31: Monitor network infrastructure with VPC Flow Logs**<br>+ Introduction<br>+ Preparation<br>+ Enable VPC Flow Logs<br>+ Monitor the network infrastructure<br>+ Clean up resources | 24/11/2026 | 24/11/2026 | [Lab 31 Intro](https://000074.awsfcaj.com/vi/1-introduce/)<br>[VPC Flow Logs](https://000074.awsfcaj.com/vi/4-enablevpcflowlogs/) |
| **Wed** | **- Practice Lab 32: Getting started with Grafana on AWS**<br>+ Introduction<br>+ Preparation<br>* Create a VPC and subnet<br>* Create a Security Group<br>* Create an EC2 Instance<br>* Create an IAM User<br>* Create an IAM Role<br>* Attach the IAM Role<br>+ Install Grafana<br>+ Monitor with Grafana<br>+ Clean up resources | 25/11/2026 | 25/11/2026 | [Lab 32 Intro](https://000029.awsfcaj.com/vi/1-introduce/)<br>[Install Grafana](https://000029.awsfcaj.com/vi/3-installgrafana/) |
| **Thu** | **- Practice Lab 33: AWS CloudWatch Workshop**<br>+ Introduction<br>+ Preparation<br>+ CloudWatch Metrics<br>* Viewing Metrics<br>* Search expressions<br>* Math expressions<br>* Dynamic Labels<br>+ CloudWatch Logs<br>* CloudWatch Logs<br>* CloudWatch Logs Insights<br>* CloudWatch Metric Filter<br>+ CloudWatch Alarms<br>+ CloudWatch Dashboards<br>+ Clean up resources | 26/11/2026 | 26/11/2026 | [Lab 33 Intro](https://000036.awsfcaj.com/vi/1-introduce/)<br>[Metrics](https://000036.awsfcaj.com/vi/3-cloudwatchmetric/)<br>[Logs](https://000036.awsfcaj.com/vi/4-cloudwatchlogs/)<br>[Alarms](https://000036.awsfcaj.com/vi/5-cloudwatchalarm/) |
| **Fri** | **- CPAWS: review project documentation and coordinate report handoff**<br>+ Cross-check the proposal, ADRs, official test2020, Rolling Accuracy and Chapters 1–5 for consistency<br>+ Confirm the FCAJ workshop Project structure with Khải; prepare Markdown, links and figures under the agreed format<br>+ Help verify the consolidated report, demo and submission materials without claiming to deploy or record the demo for others<br>**- CPAWS: verify final report and summarize Modeling & Evaluation**<br>+ Review Rolling Accuracy status, champion/challenger and remaining scientific limitations<br>+ Coordinate with the team on confirmed operational status, final cost and workshop references without claiming production ownership<br>+ Summarize personal contributions, AWS learning and lessons from reproducible forecasting evaluation | 27/11/2026 | 27/11/2026 | [GitHub Pages](https://docs.github.com/en/pages)<br>[AWS Cost Explorer](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/) |

### ACHIEVEMENTS IN WEEK 12:

1. Set strict IAM policies to control resource creation, prevent budget overruns (cost control) and ensure security.
2. Built multi-layer monitoring: network traffic with VPC Flow Logs and application metrics visualized on Grafana/CloudWatch Dashboards.
3. Cross-check the proposal, ADRs, Chapters 1–5 and official test2020 evidence before the team finalizes submission.
4. Confirm the FCAJ workshop Project structure with Khải and prepare Markdown/link checks; do not claim that the site is deployed.
5. Prepared a final review of the available forecast and accuracy evidence and recorded which production facts require team confirmation; did not claim responsibility for the live deployment.
6. Consolidated the model-evaluation methodology, artifact audit and point-in-time limitations for the individual workshop report.

