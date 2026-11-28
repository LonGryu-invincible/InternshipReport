---
title: "Week 5 Worklog"
date: 2026-10-12
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### OBJECTIVES IN WEEK 5:
- Understand and apply the Serverless architecture (AWS Lambda) to automate operations (cost optimization) and handle events (event-driven).
- Master how Lambda interacts with storage (S3) and the NoSQL database (DynamoDB).
- Master the AWS CLI to manage resources quickly and professionally instead of using only the Console.
- Review the CPAWS proposal draft and API target definitions during the 14–15 October project discussions.

### TASKS OF WEEK 5:

| Day | Task | Start Date | End Date | References |
|:---:|---|:---:|:---:|---|
| **Mon** | - Study event-driven AWS Lambda workflows, IAM permissions and CloudWatch basics to prepare for Lab 13 and Lab 14. | 12/10/2026 | 12/10/2026 | [Lab 13 Intro](https://000022.awsfcaj.com/vi/1-introduce/)<br>[Create Role](http://000022.awsfcaj.com/vi/4-createroleforlambda/)<br>[Lambda Function](https://000022.awsfcaj.com/vi/5-createlambdafunction/) |
| **Tue** | **- Practice Lab 13: Optimize EC2 costs with Lambda**<br>+ Introduction<br>+ Preparation<br>* Create a VPC<br>* Create a Security Group<br>* Create an EC2 instance<br>* Slack incoming web-hooks<br>+ Create tags for the instance<br>+ Create a role for Lambda<br>+ Create the Lambda functions<br>* Function to stop instances<br>* Function to start instances<br>+ Check the results<br>+ Clean up resources | 13/10/2026 | 13/10/2026 | [Lab 13 Intro](https://000022.awsfcaj.com/vi/1-introduce/)<br>[Create Role](http://000022.awsfcaj.com/vi/4-createroleforlambda/)<br>[Lambda Function](https://000022.awsfcaj.com/vi/5-createlambdafunction/) |
| **Wed** | **- Team project meeting: draft the proposal, define the problem statement and main web app flows**<br>+ Read the problem statement, four-asset scope, USD/VND forecast flow and chatbot requirements<br>+ Reviewed the Modeling & Evaluation requirements: log-return targets, time-based splits, baseline, pinball loss and leakage prevention<br>+ Discussed fair model evaluation methods while keeping scheduled inference practical | 14/10/2026 | 14/10/2026 | [Proposal Guide](https://workshop-sample.fcjuni.com/2-proposal/) |
| **Thu** | **- CPAWS (alongside the lab):** Reviewed `docs/api/contract.md` on session-based targets, missing sessions, quantile normalization and `prob_up`; consolidated evaluation feedback.<br>**- Practice Lab 14: Serverless - Lambda interacting with S3 and DynamoDB**<br>+ Introduction<br>+ Process and optimize image sizes on AWS<br>* Create the image processing Lambda function<br>* Create an S3 bucket<br>* Create an IAM policy for the Lambda function<br>* Test the Lambda function<br>+ Write data to Amazon DynamoDB<br>* Create and manage tables in AWS DynamoDB<br>* Create a Lambda function to write data<br>+ Clean up resources | 15/10/2026 | 15/10/2026 | [Lab 11 Intro](https://000005.awsfcaj.com/vi/1-introduce/)<br>[Create RDS](https://000005.awsfcaj.com/vi/4-create-rds/)<br>[Backup](https://000005.awsfcaj.com/vi/6-backup/)<br>[Lab 14 Intro](https://000078.awsfcaj.com/vi/1-introduce/)<br>[Resize Function](https://000078.awsfcaj.com/vi/2-resize-image-function/)<br>[DynamoDB Write](https://000078.awsfcaj.com/vi/3-write-data-to-dynaomodb/) |
| **Fri** | **- Explore a new AWS topic (alongside the lab):** Began reading about Physical AI, robot simulation and reinforcement learning; noted how cloud computing supports the training of robot control policies.<br>**- Practice Lab 15: Getting started with the AWS CLI**<br>+ Introduction<br>+ Preparation<br>+ Install the AWS CLI<br>+ Check resources via the CLI<br>+ AWS CLI with Amazon S3<br>+ AWS CLI with Amazon SNS<br>+ AWS CLI with IAM<br>+ AWS CLI with VPC<br>* AWS CLI with VPC<br>* AWS CLI with Internet Gateway<br>+ Create EC2 with the AWS CLI<br>+ Troubleshooting<br>+ Clean up resources | 16/10/2026 | 16/10/2026 | [Lab 12 Intro](https://000006.awsfcaj.com/vi/1-introduction/)<br>[Launch Template](https://000006.awsfcaj.com/vi/3-create-launch-template/)<br>[ASG](https://000006.awsfcaj.com/vi/6-create-auto-scaling-group/)<br>[Test Solutions](https://000006.awsfcaj.com/vi/7-test-solutions/)<br>[Lab 15 Intro](https://000011.awsfcaj.com/vi/1-introduce/)<br>[Install CLI](https://000011.awsfcaj.com/vi/3-installcli/)<br>[CLI with EC2](https://000011.awsfcaj.com/vi/9-ec2/) |

### ACHIEVEMENTS IN WEEK 5:

1. Deployed an automated cost-saving solution (Lab 13): used Lambda to stop/start EC2 on a schedule with Slack notifications.
2. Built a serverless image processing application (Lab 14): combined Lambda, S3 and DynamoDB to resize images automatically and store metadata.
3. Became proficient with the AWS CLI (Lab 15) for the core services (S3, EC2, VPC, IAM) without the Console.
4. Reviewed the CPAWS proposal draft and API contract, aligning the problem statement, web/chatbot flow, target definitions, quantiles and evaluation criteria.
5. Started exploring Physical AI and the role of AWS in robot simulation and training through documentation; did not run GPU experiments.

