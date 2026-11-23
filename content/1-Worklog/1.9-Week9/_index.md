---
title: "Week 9 Worklog"
date: 2026-11-02
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### OBJECTIVES IN WEEK 9:
- Get started with and master the AWS Cloud Development Kit (CDK) to define cloud infrastructure in a programming language.
- Practice deploying complex architectures (ECS, ALB, API Gateway, Serverless) with CDK and Nested Stacks.
- Strengthen the Infrastructure as Code (IaC) mindset by deploying a complete Three-Tier Architecture.
- Review Rolling Accuracy eligibility and provenance and consolidate the data-quality work documented on 2–5 November.

### TASKS OF WEEK 9:

| Day | Task | Start Date | End Date | References |
|:---:|---|:---:|:---:|---|
| **Mon** | **- Team meeting: align forecast display with evaluation semantics**<br>+ Checked q10/q50/q90, nominal 80% intervals, `prob_up` and USD/VND conversion to avoid implying guaranteed coverage<br>+ Worked on the Rolling Accuracy RFC: 56-day window, `base_date`/`target_date`, eligibility and forecasts that were actually published<br>+ Reviewed the `rolling_8w` schema and alignment between internal evaluation, DynamoDB and `/accuracy/{asset}` | 02/11/2026 | 02/11/2026 | [yfinance](https://github.com/ranaroussi/yfinance)<br>[EIA Open Data API](https://www.eia.gov/opendata/) |
| **Tue** | **- CPAWS (alongside the lab):** Reviewed Rolling Accuracy updates, cutover evidence, champion configuration and historical input provenance.<br>**- Practice Lab 19: CDK basics**<br>+ Introduction<br>+ Preparation<br>* Create an IAM Role<br>+ CDK basics<br>* Create a workspace<br>* Configure Cloud9<br>+ Create a CDK Template<br>+ Update the CDK Template<br>+ Clean up resources | 03/11/2026 | 03/11/2026 | [VPC Endpoint](https://000092.awsfcaj.com/vi/6-vpcendpointaws/)<br>[PrivateLink](https://000092.awsfcaj.com/vi/7-vpcendpointonpremise/)<br>[Peering](https://000092.awsfcaj.com/vi/8-vpcpeering/)<br>[Network Manager](https://000092.awsfcaj.com/vi/9-transitgatewaynetworkmanager/)<br>[Lab 19 Intro](https://000038.awsfcaj.com/vi/1-introduce/)<br>[CDK Basic](https://000038.awsfcaj.com/vi/3-cdkbasic/)<br>[Create Template](https://000038.awsfcaj.com/vi/4-createcdktemplate/) |
| **Wed** | **- Practice Lab 20: CDK basics - 2**<br>+ Introduction<br>+ Preparation<br>* Create an IAM Role<br>* Run an EC2 server<br>* Configure the VS Code environment<br>+ ECS, ALB and API Gateway<br>+ Lambda and S3<br>+ Nested stack<br>* Create nested stacks with CDK<br>+ Clean up resources | 04/11/2026 | 04/11/2026 | [Lab 20 Intro](https://000076.awsfcaj.com/vi/1-introduction/)<br>[ECS & ALB](https://000076.awsfcaj.com/vi/3-ecs-alb-and-api-gateway/)<br>[Nested Stack](https://000076.awsfcaj.com/vi/5-nested-stack/) |
| **Thu** | **- Team meeting: review data sources and rolling-evaluation eligibility**<br>+ Checked S3 snapshots (`raw/`, `clean/prices/`), NYSE/CME calendars, missing sessions and quality flags against leakage requirements<br>+ Reviewed provenance, idempotency, run completion and missing-forecast/upstream-failure states in Rolling Accuracy<br>+ Reviewed schema/contract changes and prepared test2020; teammates handled ingest Lambda and infrastructure implementation | 05/11/2026 | 05/11/2026 | [pandas_market_calendars](https://github.com/rsheftel/pandas_market_calendars)<br>[Lambda Container Image](https://docs.aws.amazon.com/lambda/latest/dg/images-create.html) |
| **Fri** | **- Explore a new AWS topic (alongside the lab):** Reviewed an Isaac Lab example on SageMaker; compared HyperPod and Training Jobs by launch method, checkpoints and costs, and prepared notes for Blog 1.<br>**- Practice Lab 21: Introduction to Infrastructure as Code**<br>+ Introduction<br>+ Preparation<br>+ Create a Lambda function<br>+ Create a VPC and EC2<br>+ Deploy a Three-Tier Architecture<br>* Deploy the CloudFormation Stack<br>* Test access to the Web Tier<br>* Test access to the Application Tier<br>* Test access to the Database Tier<br>+ Clean up resources | 06/11/2026 | 06/11/2026 | [Lab 19 Intro](https://000037.awsfcaj.com/vi/1-introduce/)<br>[CF Basic](https://000037.awsfcaj.com/vi/3-cloudformationbasic/)<br>[CF Advanced](https://000037.awsfcaj.com/vi/4-cloudformationadvance/)<br>[Lab 21 Intro](https://000102.awsfcaj.com/vi/1-introduction/)<br>[Create Lambda](https://000102.awsfcaj.com/vi/3-createlambda/)<br>[Three Tier](https://000102.awsfcaj.com/vi/5-threetierweb/) |

### ACHIEVEMENTS IN WEEK 9:

1. Set up the CDK working environment (Cloud9, VS Code) and deployed basic infrastructure templates.
2. Applied CDK to build advanced resources: ECS Cluster, Application Load Balancer, API Gateway and Nested Stacks.
3. Deployed a standard Three-Tier Architecture (Web, App, Database layers) entirely in code (IaC).
4. Designed/reviewed Rolling Accuracy (`rolling_8w`), evaluation keys, eligibility and provenance; checked S3 snapshots and ingest states from an evaluation perspective without claiming ingest implementation.
5. Compiled introductory notes on Isaac Lab and SageMaker in preparation for the first blog post.

