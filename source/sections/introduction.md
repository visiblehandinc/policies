# Introduction

VisibleHand, Inc ("VisibleHand") is committed to ensuring the confidentiality, privacy, integrity, and availability of all electronic protected health information (ePHI) it receives, maintains, processes and/or transmits on behalf of its Clients and Users ("Customers").

VisibleHand provides secure and compliant cloud-based software for skilled nursing and senior care providers. The VisibleHand platform ("Platform") combines electronic rounding software — a mobile application used by frontline facility staff to document safety checks and observations of residents — with real-time location system (RTLS) technology that uses wearable beacons and facility-installed gateways to verify staff proximity to residents. The Platform also includes web-based reporting and management tools used by facility and corporate staff.

As a provider of software that documents the care of residents in skilled nursing and senior care facilities, VisibleHand strives to maintain compliance, proactively address information security, mitigate risk for its Customers, and assure known breaches are completely and effectively communicated in a timely manner. The following documents address core policies used by VisibleHand to maintain compliance and assure the proper protections of infrastructure used to store, process, and transmit ePHI for VisibleHand Customers.

## License

VisibleHand HIPAA policies have been adapted from the open-source HIPAA policies originally published by Catalyze, Inc. (later Datica).

The original policies can be found [here](https://github.com/catalyzeio/policies).

The adapted policies can be found, hosted by VisibleHand, [here](https://github.com/visiblehandinc/policies).

All policies are licensed under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)

## The VisibleHand Platform

VisibleHand Customers utilize hosted software from VisibleHand to document rounding observations and related resident safety data. The Platform consists of a mobile application used on dedicated devices at Customer Facilities, RTLS beacons and gateways installed at Customer Facilities, and web-based applications for reporting and administration. All Platform services are hosted on infrastructure provided by Amazon Web Services, Inc. ("AWS"). AWS does not have insight or access into application level data and, as such, does not have the ability to secure or manage risk associated with application level vulnerabilities and security weaknesses. VisibleHand has access to data models and manages all application level configurations and security. VisibleHand makes every effort to reduce the risk of unauthorized disclosure, access, and/or breach of Customer data through network controls (VPC segmentation, security groups, TLS-only endpoints) and platform settings (encryption at rest and in transit, continuous threat detection via Amazon GuardDuty).

In the future there may be 3rd party Add-on services available as part of the VisibleHand Platform. These 3rd party, or Partner, Services will be fully reviewed by VisibleHand to assure they do not have a negative impact on VisibleHand's information security and compliance posture.

## Compliance Inheritance

VisibleHand signs business associate agreements (BAAs) with its 3rd party providers ("Providers"), including AWS. These BAAs outline VisibleHand's obligations and Provider obligations, as well as liability in the case of a breach. In providing infrastructure and managing security configurations that are a part of the technology requirements that exist in HIPAA and HITRUST, as well as future compliance frameworks, VisibleHand does not manage any aspects of compliance for Providers.

Certain aspects of compliance cannot be inherited. Because of this, VisibleHand Customers, in order to achieve full compliance, must implement certain organizational policies. These policies and aspects of compliance fall outside of the services and obligations of VisibleHand.

## Version Control

Policies were last updated September 24th, 2026.
