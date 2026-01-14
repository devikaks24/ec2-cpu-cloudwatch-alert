
# EC2 CPU Monitoring with CloudWatch & SNS

## Overview
This project demonstrates real-time monitoring of an AWS EC2 instance using
Amazon CloudWatch and SNS. Email notifications are automatically sent when
CPU usage exceeds a defined threshold.

## Project Workflow
- Launched and configured an Ubuntu EC2 instance
- Enabled 1-minute detailed monitoring in CloudWatch
- Wrote a Python script to generate CPU spikes
- Created a CloudWatch Alarm (Trigger: CPU >= 50%)
- Integrated Amazon SNS for automatic email alerts
- Validated real-time alert delivery and response flow

## How It Works
When CPU usage of the EC2 instance goes above 50%, the CloudWatch alarm
is triggered. The alarm sends a message to an SNS topic, which then
delivers an email notification to the subscribed email address.

## Tools & Services Used
- AWS EC2
- Amazon CloudWatch
- Amazon SNS
- Python
- Ubuntu Linux
- AWS Console

## Outcome
Instant email alerts were received whenever CPU usage crossed the
defined threshold, enabling proactive issue detection and faster response time.

## Key Learnings
- Real-time monitoring using CloudWatch Alarms
- Hands-on experience with AWS monitoring and alerting
- Importance of alerts in preventing downtime and improving reliability

