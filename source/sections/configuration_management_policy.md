# Configuration Management Policy

VisibleHand standardizes and automates configuration management through the use of infrastructure-as-code (AWS CDK and CloudFormation) and automated deployment pipelines (GitHub Actions), as well as documentation of all changes to production systems and networks. Infrastructure-as-code templates define all VisibleHand systems according to established and tested policies, and are used as part of our Disaster Recovery plan and process.

## Applicable Standards from the HITRUST Common Security Framework

* 06 - Configuration Management

## Applicable Standards from the HIPAA Security Rule

* 164.310(a)(2)(iii) Access Control & Validation Procedures

## Configuration Management

1. AWS CDK and CloudFormation infrastructure-as-code, deployed through GitHub Actions pipelines, is used to standardize and automate configuration management. Infrastructure definitions are version controlled in GitHub.
2. Amazon GuardDuty continuously monitors production systems for unauthorized or malicious activity, including unauthorized changes and malicious software.
3. No systems are deployed into VisibleHand environments without approval of the VisibleHand Engineering Lead.
4. All changes to production systems, network configurations, and security groups are approved by the VisibleHand Engineering Lead before they are implemented to assure they comply with business and security requirements. Additionally, all changes are tested before they are implemented in production. All changes are documented through version control (GitHub pull requests and commit history). Implementation of approved changes are only performed by authorized personnel.
5. An up-to-date inventory of systems is maintained in infrastructure-as-code definitions (version controlled in GitHub), supplemented by architecture diagrams hosted on Google Drive. All systems are categorized as production and utility to differentiate based on criticality.
6. Clocks are synchronized across all systems using NTP (provided by AWS). Modifying time data on systems is restricted.
7. All front end functionality (dashboards and portals) is separated from backend (database and application) systems by being deployed on separate services.
8. All software and systems are tested using unit tests and end to end tests.
9. All committed code is reviewed using pull requests (on GitHub) to assure software code quality and proactively detect potential security issues in development.
10. VisibleHand utilizes development and staging environments that mirror production to assure proper function.
11. VisibleHand also deploys environments locally to assure functionality before moving to staging or production.
12. VisibleHand deploys to production as needed, after changes have been tested and approved. All production deployments are executed through automated pipelines.
13. All formal change requests require unique ID and authentication (GitHub accounts with two-factor authentication).
14. Production workloads run on managed AWS services with a minimal host footprint. Malware risk is mitigated through this reduced attack surface, continuous threat detection via Amazon GuardDuty, and automated patching of managed services by AWS.
15. All production storage is encrypted at provisioning. To verify encryption is consistent and in place for all production storage, checks are performed on a quarterly basis.
