---
title: "Week 5 Worklog"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
### Week 5 Objectives:
* Study Serverless architecture on AWS using Lambda, S3, and DynamoDB.
* Build an automated image processing pipeline and log metadata into a NoSQL DynamoDB database.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 3 | - Intro to Serverless: Learn about Serverless concepts and roles of Lambda, S3, DynamoDB | 19/05/2026 | 19/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Image Optimization: Create S3 Bucket, write Lambda code to auto-compress/resize images | 20/05/2026 | 20/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Setup DynamoDB: Create a DynamoDB table and define a Partition Key | 21/05/2026 | 21/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Log data to DynamoDB: Configure Lambda function to write image metadata into DynamoDB | 22/05/2026 | 22/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 7 | - IAM Role for Lambda: Grant Least Privilege S3/DynamoDB access permissions to Lambda | 23/05/2026 | 23/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Sun | - Serverless Lab: Practice testing the full image pipeline and clean up AWS resources | 24/05/2026 | 24/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Serverless Review: Review Event-driven Architecture concepts on AWS | 25/05/2026 | 25/05/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Week 5 Achievements:
* Gained a solid understanding of Serverless and AWS Lambda trigger mechanisms.
* Developed a Lambda function to automatically resize/compress images uploaded to S3.
* Initialized a DynamoDB table and structured a NoSQL database schema.
* Integrated AWS SDK into Lambda to write image metadata records into DynamoDB.
* Implemented secure IAM policies with Least Privilege access for the Lambda function.
* Successfully executed the full Event-driven flow (S3 upload -> Lambda resize -> DynamoDB log).
* Learned best practices for cleaning up unused resources to optimize cloud costs.
