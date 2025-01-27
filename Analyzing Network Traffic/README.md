# Analyze Network Traffic

## Overview

This project focuses on analyzing network traffic and enhancing security by detecting and blocking traffic from specific IP addresses. It leverages AWS services such as Amazon VPC Flow Logs, Amazon S3, and Network Access Control Lists (NACLs) to identify and deny unauthorized access.

<p align="center">
  <img src="../../Images/project-3-architecture-diagram.png" alt="" style="display: block; margin: auto;" />
</p>

## Table of Contents

- [Requirements](#requirements)
- [Steps](#steps)
- [Conclusion](#conclusion)
- [Contributors](#contributors)

## Requirements

To complete this project, you will need an AWS account with access to the following services:

- Amazon VPC
- Amazon S3
- Amazon VPC Flow Logs
- Network Access Control Lists (NACLs)

## Steps

This project is broken down into the following steps:

1. Set up Amazon VPC Flow Logs to capture network traffic.
2. Configure Amazon S3 as the storage destination for Flow Logs.
3. Analyze the captured traffic logs to identify suspicious IP addresses.
4. Update Network ACLs to block the identified IP addresses.

### Step 1: Enable VPC Flow Logs

- Navigate to the Amazon VPC console and select the VPC you want to monitor.
- Enable VPC Flow Logs by creating a new log group and assigning it to an Amazon S3 bucket.
- Configure the log format to include relevant details, such as source and destination IP addresses.

### Step 2: Store Logs in Amazon S3

- Create an Amazon S3 bucket to store the VPC Flow Logs.
- Attach the appropriate IAM policy to grant permissions for Flow Logs to write to the S3 bucket.
- Verify that logs are being uploaded to the S3 bucket.

### Step 3: Analyze Traffic Logs

- Download the Flow Logs from the S3 bucket for analysis.
- Use tools such as Amazon Athena, Python scripts, or third-party log analysis tools to identify suspicious IP addresses or patterns.
- Compile a list of IP addresses to be blocked.

### Step 4: Update Network ACLs

- Navigate to the Amazon VPC console and locate the NACL associated with your subnet.
- Add deny rules for the identified IP addresses, specifying the protocol and port range as needed.
- Test the updated NACL to ensure that the specified IP addresses are successfully blocked.

## Conclusion

This project demonstrates how to analyze and secure network traffic using AWS services. By leveraging VPC Flow Logs, Amazon S3, and Network ACLs, you can proactively detect and block traffic from malicious IP addresses, enhancing the overall security of your AWS environment. This project is part of the AWS Cloud Quest learning path, providing hands-on experience with AWS security services.

## Contributors

[Gedion Daniel](https://gediondaniel.dev/)
[LinkedIn](https://www.linkedin.com/in/gedion-daniel-760ba6280/)
