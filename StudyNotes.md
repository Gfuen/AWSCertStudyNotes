# Cloud Concepts and Technology

## 6 Advantages of Cloud Computing 
```
-Trade Capital Expense for Variable Expense 
-Benefit from massive economies of scale 
-Stop guessing about capacity 
-Increase speed and agility 
-Stop spending money running and maintaining data centers
-Go global in minutes 
```
## 3 Types of Cloud Computing 
```
-IAAS
-PAAS 
-SAAS 
```
## Data Center 
```
-Building filled with servers 
```
## IAM Credential Report
```
-MFA
-Password Rotation
-Access keys
```
## S3
```
-Store flat files that do not change (images, videos, etc...)
-Bucket is a universal unique namespace
-Bucket is like a folder
-200 status if upload complete
-Object is key value store
    -keys (name)
    -value (data)
-Tierd
    -S3 Standard - 99.99 available
    -S3 - IA faster access but less frequent
    -S3 - Intelligent Tiering
-S3 Glacier - store any amount of data arhives
-S3 Charges
    -Storage
    -Requests
    -Transfers
-Can use s3 mb to make s3 bucket using CLI
```
## CloudFront
```
-Edge Location - Location where content will be cached. Separate from AWS Region/AZ
-Origin - Origin of all the files that the CDN will distribute
-Distribution - Name given the CDN 
-Types of Distribution 
    -Web Distribution -Websites
    -RTMP -Media Streaming 
```
## EC2
```
-On Demand - fixed rate for server
-Reserved - Provides with capacity reservation at discount. Contract Terms are 1 or 3 Yr Terms
-Spot where spot is bid price
-Dedicated host - server for your own use. Great for regulatory requirements.
-Amazon EBS volumes are placed in specific Availability Zones
```
## Load Balancers
```
-Application Load Balancers -  Layer 7 make intelligent decisions
-Network Load balancers - Static IP Addresses
-Classic Load balancers - Test & Dev, Keep costs low
```
## RDS  
```
-SQL DBS engine
-Multi Az for Disaster Recovery fails to second DB if first fails
-Read Replicas reads are copied to second DB 
-Collection - Table
-Document - Row
-Key Value Pairs - Fields
```
## Data Warehousing (RedShift)
```
-Pull in large data sets for queries usually for data analytics
```
## ElastiCache (Redis)
```
-Web service that makes it easy to deploy, operate, and scale an in-memory cache in the cloud
```
## AutoScaling
```
-Based on CPU
```
## Elastic Beanstalk 
```
-Upload zip or war and create
-deploy and manage apps
```
## AWS CloudFormation 
```
-Service that helps model and setup AWS resources
-Can create a template or use a managed template
-Can upload a template or use on from S3 
```
## Non-Relational Database (DynamoDB)
```
-Managed NoSQL DB
-No joins or complex queries
```
## Graph Database (Neptune)
```
-High AZ
-Scalable
```
## Relational Database (Aurora)
```
-Joins and queries
```
## AWS Services OnPrem
```
-Snowball
```
## AWS Systems Manager
```
-Systems Manager can be used to manage fleets of EC2 instances and Virtual machines
-Can be both inside AWS and on premise
-Run command to install, patch, uninstall software
```
## Personel Health Dashboard
```
-Overview of resources used
-Displays up to date information on AWS services and notifications
```
## EBS
```
-For storing OS and Databases
-Virtual hard disk
-Volume replicated in AZ 
-Volume size cant be changed automatically
```
## EFS Elastic File System 
```
-Doesnt come with set size
-Good for databases / file server / CMS's 
-Configure file systems easily
-Adjusts file size easily
```
## AWS Global Accerlerator
```
-Sends traffic faster for applications
-Use Amazons backbone and improve user performance
```
## Understand difference between a region, an Availability Zone and an Edge Location
```
-Region is a physical location in the world which consists of 2+ Availability Zones 
-An AZ is one more discrete data centers
-Edge locations are endpoints for AWS which are used for caching content (CDN or CloudFront)
```
## Choosing the right AWS Region
```
-Data Sovereignty Laws 
-Latency
-AWS Services 
```
## IAM
```
-Identity and Access Management is Global 
```
## Types of EBS volumes
```
-SSD 
    -GP2 
    -IO1 
-Magnetic
    -ST1 
    -SC1 
```
## Firewall
```
-Let everyting in - 0.0.0.0/0
-Single IP - X.X.X.X/32
```
## Security Groups
```
-Virtual Firewalls
```
## AWS Services can be used On-Prem  
```
-Snowball
-Snowball Edge 
-Storage Gateway
-CodeDeploy 
-Opsworks
-IOT Greengrass
```

# Billing and Pricing

## Capex vs Opex
```
-Capex -Capital Expenditure which is paid up front. Fixed sunk cost.
-Opex - Operational Expenditure which is where you pay for what you use
```
## Basic Pricing policies
```
-Pay as you go 
-Pay less when you reserve 
-Pay even less per unit by using more  
-Pay even less as AWS grows
-Custom pricing 
```
## 3 fundamental drivers of cost AWS
```
-AWS 
-Storage 
-Data Outbound
```
## AWS offers several pricing models depending on product
```
-On Demand 
-Dedicated Instances (usually means per VM softare licenses Windows Server, Microsoft SQL Server, etc...)
-Spot Instances 
-Reservations 
```
## AWS Free Services  
```
-Amazon VPC 
-Elastic Beanstalk 
-CloudFormation 
-IAM 
-Auto Scaling 
-Opsworks  
-Consolidated Billing 
```
## What Determines Price?
```
-Clock Hours of Server Time 
-Instance Type 
-Pricing Model 
-Number of Instances 
-Load Balancing 
-Detailed Monitoring
-Auto Scaling 
-Elastic IP Addresses 
-OS and Software Packages
```
## Lambda Pricing and what determines it
```
-Request pricing 
    -Free Tier 1 million requests 
    -$.02 per 1 million requests 
-Duration Pricing 
    -400,000 GB seconds per mont free, upt to 3.2 million seconds of compute time 
    -$.00001667 for every GB second used thereafter 
-Additional charges 
    -You may incur additional charges if your Lambda functionuses other AWS services or transfers
```
## EBS Pricing 
```
-Volume per GB
-Snapshots per GB 
-Data Transfer
```
## S3 Pricing 
```
-Storage class 
-Storage 
-Requests 
-Data Transfer 
```
## Glacier Pricing 
```
-Storage 
-Data Retrieval Times 
```
## Snowball 
```
-PB scale data transport solution into and out of the AWS cloud 
-Big disk to move data into AWS 
-Snowball Pricing 
    -Service fee per job 
    -Daily charge 
    -Data Transfer  
```
## RDS Pricing 
```
-Clock hours of server time 
-DB Characteristics 
-Database Purchase type 
-Number of Database Instances 
-Provisional Storage 
-Additional Storage 
-Requests 
-Deployment Type 
-Data Transfer 
```
## CloudFront pricing 
```
-Traffic Distribution 
-Requests 
-Data Transfer Out
```
## AWS Budgets
```
-Gives you ability to set custom budgets that alert you when costs exceed budgeted amount
-Used to explore costs BEFORE they have been incurred 
```
## AWS Cost Explorer
```
-Easy-to-Use interface that lets you visualize, understand, and manage your AWS costs and usage over time 
-Used to explore costs AFTER they have been incurred
```
## What level of Support do I need for a TAM?
```
-Enterpise
```
## Support Times 
```
-Basic Support Plan 
    -None 
-Developer Support Plan 
    -General Guidance: < 24 business hours 
    -System impaired: < 12 business hours 
-Business Support Plan 
    -General Guidance: < 24 business hours 
    -System impaired: < 12 business hours 
    -Porduction System impaired: < 4 hours 
    -Production System down: < 1 hour 
-Enterprise Support Plan
    -General Guidance: < 24 business hours 
    -System impaired: < 12 business hours 
    -Porduction System impaired: < 4 hours 
    -Production System down: < 1 hour 
    -Business-critical System down: < 15 minutes 
```
## Tags 
```
-Key Value Pairs attached to AWS resources
-Tags can sometimes be inherited
```
## Resource Groups (per Region basis)
```
-Make it easy to group your resources using the tags that are assigned to them
-Can group resources that share one or more tags 
-Resource groups contain information such as;
    -Region
    -Name 
    -Employee ID 
    -Department
-Using Resource Groups you can apply automation to resources tagged with specific tags
```
## Tag Editor 
```
-Tag Editor is a global service that allows use to discover resources and to add aditional tags
```
## AWS Organizations
```
-Account Management service that enables you to consolidate multiple AWS accounts into an organization that you create and centrally manage 
-2 feature sets 
    -Consolidated billing 
    -All features 
-Root account 
-Member accounts 
-Paying account is independent. Cannot access resources of the other accounts 
-All linked accounts are independent 
-Linked accounts
    -20 Linked accounts 
-Billing alerts
    -Can still create billing alerts per individual account 
    -When monitoring is enabled on the paying account, the billing data for all linked accounts is included
-Root account cannot invite another root account 
```
## Advantages of Consolidated Billing 
```
-One bill per AWS account 
-Very easy to track charges and allocate costs 
-Volume pricing discount 
```
## CloudTrail vs CloudWatch 
```
-CloudWatch monitors performance 
-CloudTrail monitors API calls in the AWS platform 
```
## CloudTrail 
```
-Per AWS account and is enabled per region
-Can consolidate logs using an S3 bucket 
    -Turn on CloudTrail in paying account
    -Create a bucket policy that allows cross-account access
    -Turn on CloudTrail in the other accounts and use the bucket in the paying account 
-Increases visibility into user and resource activity by recording API calls
```
## AWS Quick Start
```
-Way of deploying environments quickly, using CloudFormation templates built by AWS Solutions Architects who are experts
```
## AWS Landing Zone
```
-Helps customers more quickly setup a secure multi-account AWS environment based on AWS best practices
```
## AWS Partner Program
```
-Select Partner
-Advanced Partner 
-Premier Partner 
```
## AWS Calculators 
```
-AWS Simple Monthy Calculator 
    -Used to calculate your running costs on AWS on a per month basis. NOT a comparison tool.
-AWS Total Cost of Ownership Calculator 
    -Used to compare costs of running your infrastructure on premise vs in AWS Cloud. Gives report on usage that you can bring to C level execs.
```

# Security in the Cloud

## Shared Responsibility Model
```
-AWS - Responsible for Security 'OF' the Cloud such as the Hardware of Datacenters 
-Customer - Responsible for Security 'IN' the Cloud such as Patches for EC2 servers
```
## AWS WAF 
```
-Web Application Firewall protect your web applications from common web exploits 
-Protects OSI Layer 7
59 AWS Shield
-DDOS protection service that safeguards
-Two tiers 
    -Standard 
    -Advanced
```
## AWS Firewall Manager 
```
-Simplifies AWS WAF administration and maintenance tasks across multiple accounts and resources 
```
## Amazon Inspector
```
-Automated security assessment service that helps improve the security and compliance of applications deployed on AWS
-Produces detailed list of security findings
-Runs inside and inspects EC2
```
## AWS Trusted Advisor
```
-Online resource to help reduce cost, increase performance, and improve security by optimizing AWS environment
-Provides real time guidance
-Two tiers 
    -Core Checks and Recommendations
    -Full Trusted Advisor - Business and Enterprise Companies Only (upgrade plan)
```
## AWS Config 
```
-Provides a detailed view of the configuration of AWS resources
-Overview includes change in configurations over time or how they relate to one another 
-Used to monitor configurations of AWS resources 
```
## AWS Penetration Testing 
```
-You can carry out penetration tests against your AWS infrastructure without prior approval for 8 services 
    -EC2, Lambda, RDS, Aurora, etc..
```
## AWS KMS
```
-Region based service 
-Manages Customer Managed Keys 
-Ideal for S3 Objects, database passwords, and API keys stored in SSM Parameter Store 
-Encrypt and Decrypt up to 4 KB in size 
-Integrated with most of AWS Services 
-KMS is on shared hardware 
```
## AWS CloudHSM 
```
-Dedicated Hardware for you 
-Compliant with FIPS 140-3 Level 3
-Single tenant, dedicated hardware, multi-AZ cluster
```
## AWS SSM Parameter Store
```
-Secure serverless storage for configuration and secrets 
-Values can be stored encrypted(KMS) or plaintext
-Can set TTL to expire values 
-Free to sue, limit 10,000 parameters 
```
## AWS SSM Secrets Manager 
```
-Charged per secret stored and per 10,000 API calls 
-Automatically rotate secrets 
-Apply the new key/password in RDS for you 
-Generate random secrets 
-Secure secrets storage 
```
## AWS GuardDuty 
```
-Uses Machine Learning algorithms anomaly detection and third-party data to monitor and protect AWS account 
-One click to enable (30 day trial)
-Input Data includes
    -CloudTrail event logs 
    -VPC Flow logs
    -DNS logs 
```
## AWS Control Tower 
```
-Easiest way to setup and govern a new secure multi-account AWS environment
-Allows you to provision multiple AWS accounts in just a few minutes 
-Those accounts will conform to company policies 
-Used for large enterprises with multiple AWS accounts 
```
## AWS Security Hub 
```
-Comprehensive view of security alerts across multiple AWS account
-Aggregates, organizes, and prioritizes security alerts or findings 
```
## Compromised IAM credentials
```
-Determine what resources those credentials have access to 
-Invalidate the credentials so they can no longer be used to access 
-Consider invalidating any temporary security credentials 
-Restore appropritate access 
-Review access to AWS account 
```
## Athena
```
-Serverless query service which enables you to analyse and query data located in S3 using standard SQL
-Used cases 
    -Used to query log files 
    -Generate business reports 
    -Analyse AWS cost 
    -Run queries on click-stream data 
```
## Macie 
```
-Security service which uses Machine Learning and NLP to discover, classify, and protect sensitive data in S3 
-Great fro PII data
```
## AWS Artifact
```
-Used to retrieve compliance reports
```

# Advanced Concepts in the Cloud 

## Lex 
```
-AI Service that allows you to build conversational chatbots
-Powers Alexa, powered by voice or text 
```
## Poly 
```
-Powers Alexa 
-Converts text to life-like voice 
```
## Transcribe
```
-Converts speech into text 
-Can be great for generating subtitles 
```
## Recognition
```
-Converting images into tags/text 
-Upload an image and Rekognition will tell you what it thinks the image is with a certain degree of confidence 
```
## Lightsail
```
-Simple Cloud servers
-No customization like EC2 
```
## Serverless Application Repository
```
-Allows you to deploy pre-provisioned serverless applications such as Alexa Skills
```
## AWS Outposts
```
-A way of extending compute to your own data centers or on-premises
``` 
## VPC 
```
-Virutal logically isolated network to provision resources
```
## AWS Direct Connect
```
-Establish private connection between AWS and data center 
-Can reliabe secure VPN over Direct Connect 
```
## Lambda 
```
-Compute service where you can upload your code and create a lambda functionuses
-Lambda functions are triggered by events 
-Pricing    
    -1 million requests are free 
    -$0.20 per 1 million requests thereafter 
    -Duration of code run and memory used 
```











