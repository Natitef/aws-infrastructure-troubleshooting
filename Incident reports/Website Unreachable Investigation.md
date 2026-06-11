## Issue

Users reported that the hosted web application was unavailable and inaccessible through a web browser.

## Investigation

Verified that the EC2 instance was running and confirmed that the Apache web server service was active. Reviewed Security Group inbound rules to determine whether web traffic was allowed to reach the server.

## Root Cause

The HTTP inbound rule (TCP port 80) had been removed from the Security Group, preventing web traffic from reaching the EC2 instance.

## Resolution

Restored the HTTP inbound rule and verified successful access to the website through a web browser.

## Preventive Action

Implement change-control procedures and review Security Group modifications before deployment to production environments.
