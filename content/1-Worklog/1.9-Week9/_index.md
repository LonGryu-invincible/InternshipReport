---
title: "Week 9 Worklog"
date: 2026-11-09
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### OBJECTIVES IN WEEK 9:
- Practice integrating a frontend with a serverless backend using API Gateway, Lambda and DynamoDB.
- Build an automated CI/CD pipeline for serverless applications with AWS CodePipeline.
- Practice in-depth monitoring and tracing of serverless applications with CloudWatch and X-Ray.
- Finalize the model evaluation approach before official test2020; review the first Rolling Accuracy run on 12 November, align metric publication rules and retain the champion as the basis for integration and operation.
- Complete the individual article on Isaac Lab with SageMaker AI.

### TASKS OF WEEK 9:

| Day | Task | Start Date | End Date | References |
|:---:|---|:---:|:---:|---|
| **Mon** | **- Team project meeting: establish model benchmarks and evaluation**<br>+ Consolidated DLinear, CEEMDAN–DLinear/K3, K3b and S1a results and validation 2019 limitations<br>+ Checked `pinball_skill`, bootstrap confidence intervals, `baseline-q252` benchmark and criteria for confirming the existing champion<br>+ Reviewed test2020 runbook/runner: walk-forward, validity masks, DM-HAC, Holm correction and one-time official execution | 09/11/2026 | 09/11/2026 | [DLinear Paper](https://arxiv.org/abs/2205.13504)<br>[CPAWS repository](https://github.com/CPAWS-AWS-FCAJ/CPAWS-commodity-forecasting) |
| **Tue** | **- Individual Isaac Lab article (alongside the lab):** Finished an introductory post about humanoid-robot training with Isaac Lab on Amazon SageMaker AI, based on AWS documentation rather than hands-on GPU training.<br>**- Practice Lab 23: Serverless - Writing a front-end that calls API Gateway**<br>+ Introduction to API Gateway / DynamoDB<br>+ Deploy the front-end<br>+ Deploy the Lambda functions<br>* Create a table in DynamoDB<br>* Deploy the Lambda functions<br>Lambda function to write data<br>Lambda function to read data<br>Lambda function to delete data<br>+ Set up API Gateway<br>* Create the methods<br>* Configure and enable CORS<br>+ Test the API with Postman<br>+ Test the API with the front-end<br>+ Clean up resources | 10/11/2026 | 10/11/2026 | [Lab 23 Intro](https://000079.awsfcaj.com/vi/1-introduction/)<br>[Deploy Frontend](https://000079.awsfcaj.com/vi/2-front-end-deployment/)<br>[API Gateway](https://000079.awsfcaj.com/vi/4-config-api-gw/)<br>[Postman Test](https://000079.awsfcaj.com/vi/5-test-api-by-postman/)<br>[Isaac Lab documentation](https://isaac-sim.github.io/IsaacLab/)<br>[SageMaker AI documentation](https://docs.aws.amazon.com/sagemaker/) |
| **Wed** | **- CPAWS (alongside the lab):** Reviewed Chapter 2 methodology, statistical testing and the pre-lock conditions for official test2020.<br>**- Practice Lab 24: Serverless - CI/CD with CodePipeline**<br>+ Preparation<br>+ Build the SAM pipeline<br>* Create a Git repository<br>* Create the SAM pipeline<br>+ Build the front-end pipeline<br>* Create a Git repository<br>* Create the pipeline<br>+ Test the website<br>+ Clean up | 11/11/2026 | 11/11/2026 | [Lab 24 Intro](https://000084.awsfcaj.com/vi/1-preparation/)<br>[SAM Pipeline](https://000084.awsfcaj.com/vi/2-build-sam-pipeline/)<br>[CPAWS repository](https://github.com/CPAWS-AWS-FCAJ/CPAWS-commodity-forecasting) |
| **Thu** | **- Team project meeting: finalize the production model and write Lambda predict code**<br>+ Checked four `COMPLETED` jobs against API `collecting` 9/20; clarified that job completion does not mean enough samples to publish metrics<br>+ Reviewed eligible base dates, provenance and reporting data flow<br>+ Confirmed `baseline-q252` remained champion while S1a ran in shadow, without automatic promotion | 12/11/2026 | 12/11/2026 | [DynamoDB Query](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Query.html)<br>[CPAWS repository](https://github.com/CPAWS-AWS-FCAJ/CPAWS-commodity-forecasting) |
| **Fri** | **- Explore a new AWS topic (alongside the lab):** Read about EKS, AWS Batch, SageMaker and Terraform in Physical AI Toolchain; noted the roles of NVIDIA components in preparation for the Physical AI Toolchain article.<br>**- Practice Lab 25: Serverless - Monitoring serverless applications with CloudWatch and X-Ray**<br>+ Preparation<br>+ Monitoring with CloudWatch<br>* Debug with CloudWatch logs<br>* Create custom metrics<br>* Create alerts with CloudWatch Alarm<br>+ Tracing with X-Ray<br>+ Clean up | 13/11/2026 | 13/11/2026 | [Lab 25 Intro](https://000085.awsfcaj.com/vi/1-preparation/)<br>[CloudWatch](https://000085.awsfcaj.com/vi/2-cloudwatch-monitor/)<br>[X-Ray](https://000085.awsfcaj.com/vi/3-x-ray-trace/)<br>[AWS Physical AI Toolchain](https://aws.amazon.com/blogs/physical-ai/introducing-aws-physical-ai-toolchain/)<br>[Physical AI for Robotics on AWS](https://aws.amazon.com/solutions/physical-ai-for-robotics-on-aws/) |
| **Sat** | **- Attended Cloud Mastery 1: Amazon Bedrock AgentCore**<br>+ Learned about AgentCore components and how they work together in an AI agent application on AWS. | 14/11/2026 | 14/11/2026 | [Amazon Bedrock AgentCore](https://aws.amazon.com/bedrock/agentcore/)<br>[AgentCore Developer Guide](https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/what-is-bedrock-agentcore.html) |

### ACHIEVEMENTS IN WEEK 9:

1. Deployed a full-stack serverless app: connected the front-end to the back-end through API Gateway and Lambda, and handled CORS correctly.
2. Set up an automated DevOps (CI/CD) process for serverless applications, making code and front-end deployments fast and less error-prone.
3. Finalized the official test2020 evaluation approach (bootstrap, DM-HAC, Holm, validity mask) based on validation 2019 and retained `baseline-q252` as champion.
4. Reviewed the 12 November Rolling Accuracy run, clarified the difference between `COMPLETED` jobs (4/4 assets) and API `collecting` (9/20), and aligned metric publication rules and the S1a shadow role as the basis for Week 10 technical handover documentation.
5. Finished the article on Isaac Lab with SageMaker AI on 10 November and continued exploring Physical AI Toolchain.
6. Attended Cloud Mastery 1 on 14 November and learned about Amazon Bedrock AgentCore.
