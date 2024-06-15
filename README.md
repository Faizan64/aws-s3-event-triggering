# AWS-s3-Event_triggering
- AWS S3 Event triggering is a very popular project used by top organisations like netflix, amzaon, pininterest etc.
- It is a real time project using shell scripting. Services involved S3, Lambda, IAM Role, and SNS.

![event-triggering](https://github.com/Faizan64/aws-s3-eventtriggering/assets/91891601/31b35e5e-bb47-4474-919b-9234cca6c496)

## Working
- It starts with a s3 buckets whenever you upload something on the s3 bucket
- s3 will triggers the lamba function since it is a serverless compute and cheap
- Then the info is sent the SNS(Simple Notification Service) 
