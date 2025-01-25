# Highly Available Web Application on AWS
## Overview

The infrastructure implements a fault-tolerant web application that automatically scales based on demand. By leveraging AWS's global infrastructure and services, the application maintains high availability and optimal performance under varying load conditions.

## Architecture Diagram

<p align="center">
  <img src="./img/1.png" alt="" style="display: block; margin: auto;" />
</p>

## AWS Services

The infrastructure utilizes the following AWS services:

- **Amazon Route 53**: Manages DNS routing and domain configuration
- **Amazon CloudFront**: Delivers content through a global CDN network
- **Amazon S3**: Stores static assets (images, videos)
- **Elastic Load Balancer**: Distributes traffic across multiple servers
- **EC2 Auto Scaling**: Automatically adjusts server capacity based on demand
- **Amazon CloudWatch**: Monitors performance and triggers scaling actions

## Key Features

- Multi-availability zone deployment for redundancy
- Automatic scaling based on CPU utilization (threshold: 80%)
- Global content delivery through CloudFront
- Health monitoring and automated instance replacement
- Cost optimization through dynamic resource allocation

## Implementation Results

[Insert output screenshots]

## Prerequisites

- AWS Account with appropriate permissions
- Basic understanding of AWS services
- AWS CLI configured with necessary credentials

## Deployment Steps

1. Configure Auto Scaling Group with Application Load Balancer
2. Set up Load Balancer health checks
3. Enable multi-availability zone deployment
4. Configure CloudWatch monitoring

## Contributing

Contributions are welcome. Please feel free to submit a Pull Request.

## License

[Insert your license information]

## Contact

[Your contact information]
