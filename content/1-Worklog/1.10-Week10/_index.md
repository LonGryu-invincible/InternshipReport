---
title: "Week 10 Worklog"
date: 2026-11-09
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### OBJECTIVES IN WEEK 10:
- Master end-to-end serverless architecture: from event processing (S3 triggers) and storage (DynamoDB) to building APIs (API Gateway).
- Build an automated CI/CD pipeline for serverless applications with AWS CodePipeline.
- Practice in-depth monitoring and tracing of serverless applications with CloudWatch and X-Ray.
- Review the test2020 runbook and the first Rolling Accuracy run on 12 November; complete Blog 1.

### TASKS OF WEEK 10:

| Day | Task | Start Date | End Date | References |
|:---:|---|:---:|:---:|---|
| **Mon** | **- Team meeting: review baselines/challengers and test2020 plan**<br>+ Consolidated DLinear, CEEMDAN–DLinear/K3, K3b and S1a results and validation 2019 limitations<br>+ Checked `pinball_skill`, bootstrap confidence intervals, `baseline-q252` benchmark and the decision to retain the champion<br>+ Reviewed test2020 runbook/runner: walk-forward, validity masks, DM-HAC, Holm correction and one-time official execution<br>**- Practice Lab 22: Serverless - Lambda interacting with S3 and DynamoDB**<br>+ Introduction<br>+ Process and optimize image sizes on AWS<br>* Create the image processing Lambda function<br>* Create an S3 bucket<br>* Create an IAM policy for the Lambda function<br>* Test the Lambda function<br>+ Write data to Amazon DynamoDB<br>* Create and manage tables in AWS DynamoDB<br>* Create a Lambda function to write data<br>+ Clean up resources | 09/11/2026 | 09/11/2026 | [DLinear Paper](https://arxiv.org/abs/2205.13504)<br>[Lab 22 Intro](https://000078.awsfcaj.com/vi/1-introduce/)<br>[Resize Function](https://000078.awsfcaj.com/vi/2-resize-image-function/)<br>[DynamoDB Write](https://000078.awsfcaj.com/vi/3-write-data-to-dynaomodb/) |
| **Tue** | **- Blog 1 (alongside the lab):** Finished an introductory post about humanoid-robot training with Isaac Lab on Amazon SageMaker AI, based on AWS documentation rather than hands-on GPU training.<br>**- Practice Lab 23: Serverless - Writing a front-end that calls API Gateway**<br>+ Introduction to API Gateway / DynamoDB<br>+ Deploy the front-end<br>+ Deploy the Lambda functions<br>* Create a table in DynamoDB<br>* Deploy the Lambda functions<br>Lambda function to write data<br>Lambda function to read data<br>Lambda function to delete data<br>+ Set up API Gateway<br>* Create the methods<br>* Configure and enable CORS<br>+ Test the API with Postman<br>+ Test the API with the front-end<br>+ Clean up resources | 10/11/2026 | 10/11/2026 | [Lab 19 Intro](https://000038.awsfcaj.com/vi/1-introduce/)<br>[CDK Basic](https://000038.awsfcaj.com/vi/3-cdkbasic/)<br>[Create Template](https://000038.awsfcaj.com/vi/4-createcdktemplate/)<br>[Lab 23 Intro](https://000079.awsfcaj.com/vi/1-introduction/)<br>[Deploy Frontend](https://000079.awsfcaj.com/vi/2-front-end-deployment/)<br>[API Gateway](https://000079.awsfcaj.com/vi/4-config-api-gw/)<br>[Postman Test](https://000079.awsfcaj.com/vi/5-test-api-by-postman/) |
| **Wed** | **- CPAWS (alongside the lab):** Reviewed Chapter 2 methodology, statistical testing and the pre-lock conditions for official test2020.<br>**- Practice Lab 24: Serverless - CI/CD with CodePipeline**<br>+ Preparation<br>+ Build the SAM pipeline<br>* Create a Git repository<br>* Create the SAM pipeline<br>+ Build the front-end pipeline<br>* Create a Git repository<br>* Create the pipeline<br>+ Test the website<br>+ Clean up | 11/11/2026 | 11/11/2026 | [Lab 20 Intro](https://000076.awsfcaj.com/vi/1-introduction/)<br>[ECS & ALB](https://000076.awsfcaj.com/vi/3-ecs-alb-and-api-gateway/)<br>[Nested Stack](https://000076.awsfcaj.com/vi/5-nested-stack/)<br>[Lab 24 Intro](https://000084.awsfcaj.com/vi/1-preparation/)<br>[SAM Pipeline](https://000084.awsfcaj.com/vi/2-build-sam-pipeline/) |
| **Thu** | **- Team meeting: review the first Rolling Accuracy run and evaluation contract**<br>+ Checked four `COMPLETED` jobs against API `collecting` 9/20; clarified that job completion does not mean enough samples to publish metrics<br>+ Reviewed eligible base dates, provenance and reporting data flow<br>+ Confirmed `baseline-q252` remained champion while S1a ran in shadow, without automatic promotion | 12/11/2026 | 12/11/2026 | [DynamoDB Query](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Query.html) |
| **Fri** | **- Explore a new AWS topic (alongside the lab):** Read about EKS, AWS Batch, SageMaker and Terraform in Physical AI Toolchain; noted the roles of NVIDIA components in preparation for Blog 2.<br>**- Practice Lab 25: Serverless - Monitoring serverless applications with CloudWatch and X-Ray**<br>+ Preparation<br>+ Monitoring with CloudWatch<br>* Debug with CloudWatch logs<br>* Create custom metrics<br>* Create alerts with CloudWatch Alarm<br>+ Tracing with X-Ray<br>+ Clean up | 13/11/2026 | 13/11/2026 | [Lab 21 Intro](https://000102.awsfcaj.com/vi/1-introduction/)<br>[Create Lambda](https://000102.awsfcaj.com/vi/3-createlambda/)<br>[Three Tier](https://000102.awsfcaj.com/vi/5-threetierweb/)<br>[Lab 25 Intro](https://000085.awsfcaj.com/vi/1-preparation/)<br>[CloudWatch](https://000085.awsfcaj.com/vi/2-cloudwatch-monitor/)<br>[X-Ray](https://000085.awsfcaj.com/vi/3-x-ray-trace/) |

### ACHIEVEMENTS IN WEEK 10:

1. Built a complete serverless back-end flow: automated image processing with an S3 trigger and NoSQL data management with DynamoDB.
2. Deployed a full-stack serverless app: connected the front-end to the back-end through API Gateway and Lambda, and handled CORS correctly.
3. Set up an automated DevOps (CI/CD) process for serverless applications, making code and front-end deployments fast and less error-prone.
4. Consolidated validation 2019 and test2020 preflight (bootstrap, DM-HAC, Holm, validity mask), reviewed the 12 Nov Rolling Accuracy run, and retained `baseline-q252` as champion.
5. Finished Blog 1 on 10 Nov about Isaac Lab on SageMaker AI and continued exploring Physical AI Toolchain.

