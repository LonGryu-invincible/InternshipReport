---
title: "Week 4 Worklog"
date: 2026-09-28
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### OBJECTIVES IN WEEK 4:
- Master Amazon EC2: manage the instance lifecycle, create Custom AMIs, troubleshoot and recover data.
- Practice deploying real web applications (LAMP stack, Node.js) on both Linux and Windows.
- Understand storage services (S3, Storage Gateway) and the Shared Responsibility Model.
- Review AWS security services (IAM, Cognito, AWS Organizations, KMS) and participate in the community events on 29 September and 2 October.

### TASKS OF WEEK 4:

| Day | Task | Start Date | End Date | References |
|:---:|---|:---:|:---:|---|
| **Mon** | **- Practice Lab 9: Amazon Elastic Compute Cloud (EC2)**<br>+ Introduction<br>+ Preparation:<br>* Create a Linux VPC<br>* Create a Windows VPC<br>* Create a Linux Security Group<br>* Create a Windows Security Group<br>+ Launch a Windows instance<br>* Create the Windows Instance<br>* Connect to the Windows instance<br>+ Launch a Linux instance<br>* Create the Linux instance<br>* Connect to the Linux instance | 28/09/2026 | 28/09/2026 | [Lab 9 Intro](https://000004.awsfcaj.com/vi/1-introduce/)<br>[Lab 9 Prereq](https://000004.awsfcaj.com/vi/2-prerequiste/)<br>[Launch Windows](https://000004.awsfcaj.com/vi/3-launchwindowsinstance/)<br>[Launch Linux](https://000004.awsfcaj.com/vi/4-launchlinuxinstance/) |
| **Tue** | **- Attended AWS Cloud and AI Day Hanoi — Ho Chi Minh City Watch Party**<br>**- Team project meeting: agree on the topic and divide responsibilities**<br>+ Reviewed CPAWS scope: gold, silver, Brent and WTI; 1–7 trading-session forecasts, USD/VND display and an explanatory chatbot<br>+ Took the Modeling & Evaluation role: baselines/challengers, evaluation design and result verification; collaborated with Khải as Research Lead<br>**- Continue Lab 9:**<br>+ Amazon EC2 basics<br>* Change the EC2 configuration<br>* Create an EC2 snapshot<br>* Create a Custom AMI<br>* Launch an instance from the custom AMI<br>* Access EC2-Windows after losing the Key Pair using SSM<br>* Access EC2-Linux after losing the Key Pair using User Data<br>* Configure a desktop interface for EC2-Ubuntu 22.04<br>* Amazon EBS Snapshots Archive<br>* Share an AMI | 29/09/2026 | 29/09/2026 | [Event Agenda](https://aws.amazon.com/vi/events/cloud-day-hanoi/)<br>[Amazon Bedrock](https://aws.amazon.com/bedrock/)<br>[EIA Open Data API](https://www.eia.gov/opendata/)<br>[EC2 Basic](https://000004.awsfcaj.com/vi/5-amazonec2basic/) |
| **Wed** | **- Continue Lab 9:**<br>+ Deploy a Node.js application on Amazon Linux<br>* Install a LAMP web server (preparation, testing, database configuration, phpMyAdmin installation)<br>* Install Node.js on Linux<br>* Deploy the application on the Linux instance<br>+ Node.js application on Amazon EC2 Windows<br>* Install XAMPP on the Windows instance<br>* Install Node.js on the Windows instance<br>* Deploy the application on the Windows instance<br>+ Limit resource usage with IAM<br>* Allow services only in a specific Region<br>* Limit EC2 usage by Instance Family<br>* Limit EC2 usage by Instance type<br>* Limit the EBS volume storage type<br>* Limit resource deletion by the company IP address<br>* Limit resource deletion by time window<br>+ Clean up resources | 30/09/2026 | 30/09/2026 | [Linux App](https://000004.awsfcaj.com/vi/6-awsfcjmanagement-linux/)<br>[Windows App](https://000004.awsfcaj.com/vi/7-awsfcjmanagement-windows/)<br>[Governance](https://000004.awsfcaj.com/vi/8-costusagegovernance/)<br>[Cleanup](https://000004.awsfcaj.com/vi/9-cleanup/) |
| **Thu** | **- Study Module 04: Storage services on AWS:**<br>+ 04-01: Amazon Simple Storage Service (S3) - Access Point - Storage Class<br>+ 04-02: S3 Static Website & CORS - Control Access - Object Key & Performance - Glacier<br>+ 04-03: Snow Family - Storage Gateway - Backup | 01/10/2026 | 01/10/2026 | [04-01](https://youtu.be/_yunukwcAwc?si=6HqDHVQJq8Ks9aWh)<br>[04-02](https://youtu.be/mPBjB6Ltl_Q?si=OITIt1x3d7OZ4ei_)<br>[04-03](https://www.youtube.com/watch?v=YXn8Q_Hpsu4) |
| **Fri** | **- Attend event: Meet Dr. Werner (AWS CTO) with the AWS FCAJ HCM community**<br>**- Study Module 05: Security services on AWS:**<br>+ 05-01: Shared Responsibility Model<br>+ 05-02: AWS Identity and Access Management<br>+ 05-03: Amazon Cognito<br>+ 05-04: AWS Organizations<br>+ 05-05: AWS IAM Identity Center<br>+ 05-06: AWS Key Management Service<br>+ 05-07: AWS Security Hub | 02/10/2026 | 02/10/2026 | [03-01](https://www.youtube.com/watch?v=-t5h4N6vfBs)<br>[03-01-01](https://www.youtube.com/watch?v=e7XeKdOVq40)<br>[03-01-02](https://www.youtube.com/watch?v=yAR6QRT3N1k)<br>[03-01-03](https://www.youtube.com/watch?v=hKr_TfGP7NY)<br>[03-01-04](https://www.youtube.com/watch?v=6IHNDJ85aoQ)<br>[03-01-05](https://www.youtube.com/watch?v=_v_43Wi7zjo)<br>[03-01-06](https://www.youtube.com/watch?v=Ew3QRaKJQSA)<br>[03-01-07](https://www.youtube.com/watch?v=bbLcPitXJSY)<br>[03-02](https://youtu.be/hFVYG8WqfU0?si=pwMJL01CuoVoxMQS)<br>[05-01](https://youtu.be/tsobAlSg19g?si=-xSAVT8MZReV10RP)<br>[05-02](https://youtu.be/N_vlJGAqZxo?si=KxeWofBCdviRYax1)<br>[05-03](https://youtu.be/pZ2fgEFK3Vs?si=QWkbW4avA9wlvlhP)<br>[05-04](https://youtu.be/5oQY8Rogz9Y?si=WK72gwmztbXWQVKr)<br>[05-05](https://youtu.be/NW1xrMkNMjU?si=Owp-3CDDmW7YYTY4)<br>[05-06](https://youtu.be/GMihNQojhZc?si=Bt4oUqD2a5_IA0mm)<br>[05-07](https://youtu.be/clj2E0rNBEs?si=eUp1O-14XFDbpbbe) |

### ACHIEVEMENTS IN WEEK 4:

1. Fully completed Lab 9: proficient in advanced EC2 administration tasks (resize, snapshot, Custom AMI, recovery access).
2. Successfully deployed real applications (LAMP stack, Node.js) on EC2 Linux and Windows.
3. Mastered Module 04 on data storage solutions (S3, Glacier, Storage Gateway) and backup strategies.
4. Consolidated Module 05 on cloud security: the Shared Responsibility Model and identity tools (IAM, Cognito, Identity Center).
5. Helped settle the CPAWS idea (commodity forecasts with an explanatory chatbot) and took the Modeling & Evaluation responsibility for model comparison and result verification.
6. Learned about the agentic AI trend and the AWS "builder" mindset by attending two AWS events.

