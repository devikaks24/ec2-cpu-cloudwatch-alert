# EC2 CPU CloudWatch Alarm with SNS Email Notification

## Overview
This project uses AWS CloudFormation to create:
- An SNS Topic for CPU alerts
- Email subscription for notifications
- CloudWatch Alarm for EC2 CPU >= 50%

## How it works
- When CPU usage of the EC2 instance goes above 50%, the alarm triggers.
- An email notification is sent to the subscribed email via SNS.

## Deployment
1. Make sure AWS CLI is configured on your system.
2. Deploy the CloudFormation stack:

```bash
aws cloudformation deploy \
  --template-file cloudwatch-ec2-cloudwatch-alert.yaml \
  --stack-name ec2-cpu-alert-demo \
  --parameter-overrides AlertEmail=youremail@example.com
