---
title: "Event 3"
date: 2026-11-14
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Event 3 — Cloud Mastery 1: Amazon Bedrock AgentCore

## 1. Event Overview

- **Date:** November 14, 2026
- **Location:** 26th Floor, Bitexco Financial Tower, District 1, Ho Chi Minh City, Vietnam
- **Format:** Technical knowledge-sharing session
- **Role:** Attendee
- **Main Topic:** Amazon Bedrock AgentCore

Cloud Mastery 1 was a technical session about building and operating AI agent applications on AWS. The main topic was Amazon Bedrock AgentCore, a collection of services designed to support the deployment and operation of Agentic AI applications.

I was interested in this event because most of my previous AI studies had focused on models and algorithms. AgentCore introduced another perspective: how an AI agent can use tools, manage context, and operate within a real system.

## 2. Key Highlights

### 2.1. AI in Enterprise Applications

The opening discussion focused on the role of AI in enterprise products. One point that stood out to me was that AI does not necessarily need to be the entire product. In many applications, a model handles only part of the work, while other components manage data, users, and application features.

Previously, when experimenting with models, I mostly focused on inputs and outputs. This topic helped me understand that deploying AI in a real product involves many responsibilities beyond the model itself.

### 2.2. Main Components of Amazon Bedrock AgentCore

Based on the session and official AWS documentation, I explored the main components of AgentCore:

**AgentCore Runtime** provides a managed environment for deploying and running AI agents. It reduces the need for developers to build and maintain their own servers.

**AgentCore Gateway** allows agents to connect to external tools and services, such as APIs and AWS Lambda functions. This is important because agents may need to retrieve information or complete tasks through tools rather than simply generate responses.

**AgentCore Memory** helps manage information and context during interactions. I found this useful for applications that need to maintain information across multiple steps instead of treating every request as independent.

**AgentCore Identity** supports authentication and identity management when agents interact with other systems. This helped me understand why appropriate access controls are important, especially when agents use tools on behalf of users.

**AgentCore Observability** supports monitoring agent activities, investigating issues, and understanding system behavior. This component stood out to me because an AI system needs not only to produce results but also to provide ways to examine how those results were generated.

### 2.3. Additional Capabilities

Official AWS documentation also describes tools such as:

- **Code Interpreter:** Supports code execution for suitable tasks.
- **Browser:** Allows agents to interact with web applications through a managed browser environment.

These tools extend the capabilities of AI agents beyond the basic question-and-answer functionality of traditional chatbots.

## 3. Personal Experience

What interested me during Cloud Mastery 1 was how the different AgentCore components could work together to form a complete system.

Previously, I had spent much of my machine learning studies on data processing, model selection, and performance evaluation. As a result, topics such as execution environments, access management, and agent monitoring offered a new perspective.

After the session, I continued exploring the official AWS documentation to better understand the purpose of each component. I also realized that an Agentic AI application does not necessarily need every available service from the beginning. The choice of components should depend on the project's goals and scope.

## 4. Lessons Learned and Future Plans

My main takeaway was that **building an AI agent involves more than choosing a suitable foundation model**. A practical system also needs execution environments, tool integration, context management, access control, and monitoring.

In the future, I would like to develop an AI agent project using Amazon Bedrock AgentCore components. My goal is to explore Runtime, Gateway, Memory, Identity, and Observability step by step, then experiment with combining them in an application that can handle multi-step tasks and interact with external services.

This is a future learning goal rather than a system I have already developed or deployed.

## 5. Evidence of Participation

![Photo taken at Cloud Mastery 1 on Amazon Bedrock AgentCore](/images/4-Event/anh_event_3.jpg)



## 6. References

- [Amazon Bedrock AgentCore — AWS](https://aws.amazon.com/bedrock/agentcore/)
- [Amazon Bedrock AgentCore Developer Guide](https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/what-is-bedrock-agentcore.html)
