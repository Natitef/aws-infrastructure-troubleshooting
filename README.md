# AWS Infrastructure Troubleshooting Project

## Overview

This project simulates real-world cloud infrastructure incidents commonly handled by Technical Support Engineers, Application Support Engineers, and Cloud Support Associates.

The project focuses on identifying, investigating, and resolving AWS service issues using structured troubleshooting methodologies, root-cause analysis, and technical documentation.

AWS services used include Amazon EC2, IAM, Security Groups, and S3.

## Technologies Used

* Amazon Web Services (AWS)
* Amazon EC2
* AWS IAM
* Amazon S3
* Security Groups
* Linux (Amazon Linux 2023)
* Apache HTTP Server
* Networking Fundamentals

## Incident 1: EC2 Connection Failure

### Scenario

An EC2 instance became inaccessible through SSH.

### Investigation

* Reviewed instance status and health checks
* Verified network configuration
* Examined Security Group inbound rules
* Tested connectivity using EC2 Instance Connect

### Root Cause

The SSH inbound rule (TCP port 22) was removed from the Security Group, preventing remote access.

### Resolution

Restored the SSH rule and verified successful connectivity.

## Incident 2: IAM Access Denied

### Scenario

An IAM user was unable to access required S3 resources.

### Investigation

* Reviewed IAM user configuration
* Analyzed attached policies and permissions
* Validated S3 access requirements

### Root Cause

The IAM user did not have an S3 access policy assigned.

### Resolution

Attached the appropriate S3 permissions and verified access.

## Incident 3: Website Unreachable

### Scenario

A web application hosted on an EC2 instance became unavailable.

### Investigation

* Verified EC2 instance status
* Confirmed Apache service was running
* Reviewed Security Group inbound rules
* Tested website accessibility

### Root Cause

HTTP traffic (TCP port 80) was blocked after the inbound HTTP rule was removed.

### Resolution

Restored the HTTP Security Group rule and verified successful website access.

## Skills Demonstrated

* Cloud Infrastructure Troubleshooting
* AWS Security Group Management
* IAM Permission Analysis
* Linux Administration
* Apache Web Server Configuration
* Root Cause Analysis
* Technical Documentation
* Incident Response
* Network Troubleshooting
* Access Control Management

## Business Impact

This project demonstrates practical cloud support workflows used to investigate service outages, connectivity issues, access control problems, and application availability incidents within AWS environments.

The troubleshooting process follows a structured approach:

1. Identify the issue
2. Investigate affected components
3. Determine root cause
4. Implement corrective actions
5. Document findings and preventative measures

These activities closely mirror responsibilities performed by Technical Support Engineers, Application Support Engineers, and Cloud Support Associates in production environments.
