## Issue

Unable to establish an SSH connection to an Amazon EC2 instance.

## Investigation

Reviewed the instance status, network configuration, and Security Group rules associated with the EC2 instance.

## Root Cause

The inbound SSH rule (TCP port 22) was removed from the Security Group, preventing incoming SSH connections.

## Resolution

Restored the SSH inbound rule and verified successful connectivity using EC2 Instance Connect.

## Preventive Action

Implement change management procedures and review Security Group modifications before deployment to production environments.
