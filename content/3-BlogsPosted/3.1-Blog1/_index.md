---
title: "AI Gateway – Managing AI on AWS"
date: 2026-06-29
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---
# AI Gateway – Managing AI on AWS with Amazon Bedrock and Amazon API Gateway

As generative AI applications become widely used in enterprises, allowing direct access to AI models for every system can lead to challenges such as difficulties in cost control, lack of authorization mechanisms, and hard-to-track usage metrics.

To address this issue, AWS proposes the AI Gateway pattern, utilizing Amazon API Gateway as an intermediary layer between users and Amazon Bedrock. This architecture helps enterprises manage access control, apply request throttling, monitor costs, and enhance security when deploying Generative AI applications.

This pattern uses Amazon API Gateway as the front-end access layer for Amazon Bedrock. The solution supports key capabilities such as user authentication and authorization via existing identity systems (e.g., JWT), usage quota management, request throttling, API lifecycle management, canary releases, and integration with AWS WAF for enhanced security.

Additionally, API Gateway supports real-time response streaming, allowing foundation model outputs to stream directly to users as they are generated, rather than waiting for the entire response to complete.

Thanks to these capabilities, the AI Gateway not only acts as an entry point to Amazon Bedrock but also helps enterprises control costs, enhance security, and govern AI usage more effectively at scale.

## AI Gateway Architecture

The reference architecture gives you granular control over LLM access using fully managed AWS services. It is transparent to client applications and seamlessly integrates into existing enterprise environments.

![AI Gateway Reference Architecture](/images/3-BlogsPosted/3.1-Blog1/ai-gateway-diagram.png)
*Figure 1. Reference architecture of the AI gateway.*

The solution consists of four core components:

* **Amazon Route 53:** Manages custom domain routing, allowing clients to access the AI Gateway through a company-specific endpoint instead of the default Amazon API Gateway domain. This makes the system more professional and easier to integrate into existing infrastructure.
* **Amazon API Gateway:** Serves as the Entry Point for all requests. It provides crucial capabilities like authorization, request throttling, lifecycle management, rate limiting, and monitoring, helping enterprises control access, manage request traffic, monitor system activity, and ensure stability and security.
* **AWS Lambda Authorizer:** Handles request authorization, which in the Dynatrace implementation involves validating JWT tokens with existing authentication systems. For your specific deployment needs, you can implement custom authorization logic in a Lambda authorizer, integrate with Amazon Cognito User Pools, or use other API Gateway authorization mechanisms.
* **Lambda Integration:** A dynamic request forwarder that signs incoming requests with AWS credentials (AWS SigV4) and routes them to the appropriate Amazon Bedrock endpoints. This component preserves all details of the original request, including the API action and parameters, to support current and future Amazon Bedrock APIs without code changes. The complete implementation is provided in the Integration Lambda Function.
* **Amazon Bedrock:** Provides access to foundation models and AI capabilities.

The benefit of this architecture is the transparency to client applications and its future-proof design. Clients can use AWS SDKs (such as Boto3) to access Amazon Bedrock functionalities (such as LLMs and Knowledge Bases) exactly as they would when calling the Amazon Bedrock API directly. Meanwhile, the AI Gateway handles authorization, quota management, and other capabilities behind the scenes.

## Conclusion

The AI gateway pattern demonstrated in this post provides a scalable way to manage access to foundation models and agent tools through Amazon Bedrock. Initially developed and implemented by Dynatrace to serve their global user base, this pattern has proven its effectiveness at enterprise-scale. By using the Amazon API Gateway enterprise features, organizations can implement necessary controls while maintaining the benefits of serverless architecture.

---

* **Original article link:** [Building an AI Gateway to Amazon Bedrock with Amazon API Gateway](https://aws.amazon.com/blogs/architecture/building-an-ai-gateway-to-amazon-bedrock-with-amazon-api-gateway/)