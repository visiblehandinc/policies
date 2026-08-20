# IDS Policy

In order to preserve the integrity of data that VisibleHand stores, processes, or transmits for Customers, VisibleHand implements strong intrusion detection tools and policies to proactively track and retroactively investigate unauthorized access. VisibleHand currently utilizes Amazon GuardDuty for continuous threat detection across its AWS environment, monitoring account activity, network traffic, and data access patterns for malicious or unauthorized behavior.

## Applicable Standards from the HITRUST Common Security Framework

* 09.ab - Monitoring System Use
* 06.e - Prevention of Misuse of Information
* 10.h - Control of Operational Software

## Applicable Standards from the HIPAA Security Rule

* 164.312(b) - Audit Controls

## Intrusion Detection Policy

* Amazon GuardDuty is used to monitor and correlate account activity, network flow, and data access logs on an ongoing basis. GuardDuty findings are reviewed by the Security Officer on a monthly basis.
* GuardDuty generates alerts to analyze and investigate suspicious activity or suspected violations. High-severity findings generate automated notifications to the engineering team.
* Automatic monitoring is done to identify patterns that might signify the lack of availability of certain services and systems (DOS attacks).
* VisibleHand network controls (AWS security groups, VPC network ACLs, and AWS managed load balancing) restrict and monitor all incoming traffic. Additionally, AWS actively monitors its network to detect and absorb denial of service attacks (AWS Shield).
* All new security group rules and network configuration changes are tested before being pushed into production. Security group and network rules are reviewed every quarter.
* Network perimeters are defined and enforced using AWS VPC segmentation and security groups.
