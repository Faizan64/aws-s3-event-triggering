# AWS-s3-Event_triggering
- AWS S3 Event triggering is a very popular project used by top organizations like Netflix, amazon, Airnb etc.
- AWS Services involved S3, Lambda, IAM Role, and SNS.

![event-triggering](https://github.com/Faizan64/aws-s3-eventtriggering/assets/91891601/31b35e5e-bb47-4474-919b-9234cca6c496)

## Working
- It starts with a s3 buckets whenever new video/series/documentary is uploaded in S3 Storage
 Bucket, you receive a notification/E-mail 
- The process starts with s3 triggering the lambda function. why lambda since it is a serverless compute, can be run in any programming language and it is cheap
- Then the info is sent to the SNS(Simple Notification Service). SNS provides reliable message delivery, scalability, and fault tolerance is responsible for sending mails or notifications
- IAM(Identity and access management) allows you to create and manage roles. In this project
Hence we will need to grant IAM permission to Lambda Function. Lambda function needs to have permission to be invoked by S3 Bucket and invoke SNS. 

## Steps
- You can launch and ec2 instance or you can also use AWS CLI in my case since we have no use ec2 service I prefer to use CLI
- Get a terminal Install and configure AWS CLI(https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) with this link you can download or update your CLI
- In order to configure your CLI you need to create an secret key you can follow this path(aws console/Profile/security credentials/Access key/Create Access key.
- With AWS configure provide key id and access id and region and output put as default and your are ready to use CLI
- Clone the repo
- Execute the script
- When the execution is done all the services are created

## 1. S3 bucket

![S3 bucket](https://github.com/Faizan64/aws-s3-eventtriggering/assets/91891601/7ae9f3df-c2f4-4450-a5af-1ed53e6834bd)

## 2. IAM Roles 

![IAM roles](https://github.com/Faizan64/aws-s3-eventtriggering/assets/91891601/039c3a0e-fe90-4692-ba6f-ba2582bbdcd6)

## 3. SNS 

![SNS](https://github.com/Faizan64/aws-s3-eventtriggering/assets/91891601/295b1e5c-18cc-4763-bb39-bd29c27335b8)

## 4. Lambda Function

![lamda_fuction](https://github.com/Faizan64/aws-s3-eventtriggering/assets/91891601/a405f7d4-26ce-4836-b3a3-08c3d5e2a931)

## 5. Email Notification (subscription confirmation and notification about data upload)

![email](https://github.com/Faizan64/aws-s3-eventtriggering/assets/91891601/7b7f393e-fb01-467b-a30b-4fd094c5fd86)


  

  
