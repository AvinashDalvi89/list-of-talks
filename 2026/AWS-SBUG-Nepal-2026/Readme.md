
# Building for Scale: How to Choose the Right AWS Services as Your Product Evolves

**Event:** AWS Student Builder Group at GCES (online)
**Date:** Saturday, 21 November 2026, 7:15 PM IST (7:30 PM NPT)
**Speaker:** Avinash Dalvi, AWS Serverless Hero · Technical Architect at Quantiphi
**Audience:** Students and beginners, no prior AWS knowledge needed
**Level:** Beginner

## About the talk

You don't need to learn 200 AWS services to build a real product. This talk
starts with one app on one server and grows it step by step. Each time the app
hits a problem, we pick the simplest AWS service that fixes it.

The goal is to leave with a way to choose services, not a list to memorise.

## What we cover

**The app grows, one problem at a time**

| Problem | AWS service |
|---|---|
| Run the app | Amazon EC2 |
| Data gets lost or grows | Amazon RDS |
| Photos and videos fill the server | Amazon S3 |
| Too many users at once | Elastic Load Balancing, EC2 Auto Scaling |
| Slow for users far away | Amazon CloudFront |
| One slow step blocks everything | Amazon SNS, Amazon SQS |
| Who is allowed to do what | AWS IAM |

**How to choose**

- Three questions to ask before adding any service
- Where should my code run? EC2, Lambda, Fargate or EKS
- Where should my data live? RDS, DynamoDB or S3
- Which stage is your product in? Just launched, growing or scaling

**Where to go next:** CodePipeline, CloudFormation, CloudWatch, and setting a
billing alert before anything else.

## Key takeaways

1. Start small. Add a service only when your app has a problem that needs it.
2. Name the problem first, then pick the simplest service that fixes it.
3. Check the cost and set a billing alert at every stage.
4. Ask "Why this way?" about every choice.

## Resources

[Slides](https://github.com/AvinashDalvi89/list-of-talks/blob/main/2026/AWS-SBUG-Nepal-2026/Building%20for%20Scale.pdf)
 
