# Project SLEDGEHammer Charter

## Executive Summary

State (S), local (L), education (ED), government enterprises (GE) , and healthcare (H) organizations (SLEDGEH) are looking to expand their use of cloud native, Kubernetes-based platform services. Project SLEDGEHammer proposes to:

1.  Accelerate the adoption of cloud native services in SLEDGEH enterprises by providing a package of audited and hardened Kubernetes multi-cluster infrastructure and control plane code;
    
2.  Provide an assessment report and audited documentation and compliance-as-code artifacts that SLEDGEH enterprises can use immediately in an authorized, e.g. FedRAMP High, cloud or on-prem Kubernetes-based infrastructure, or for agency managed infrastructure, for an internal agency to authorization; and
    
3.  Provide participating CNCF community members and open source contributors greater access to SLEDGEH stakeholders, users and buyers and their application use cases.
    
## Detailed Overview

State (S), local (L), education (ED), government enterprises (GE) , and healthcare (H) organizations are looking to modernize their IT infrastructure, accelerate value delivery to mission stakeholders and end users, and adapt to evolving staffing challenges - while facing evolving and well-funded adversarial threats.

Deploying modern, cloud native, container-based devops tooling, CI/CD and data pipelines, and operational automation to scale up and out - while establishing a secure baseline and maintaining an Authority to Operate with Continuous Monitoring - is an enormously complex journey that is beyond the current capabilities for most smaller SLEDGEH entities.

Project SLEDGEHammer offers a secure, audit-ready reference architecture and necessary machine readable compliance artifacts for Kubernetes and the constellation of supporting CNCF projects that provide minimal Dev(Sec)Ops capabilities to develop, test, secure, deploy, operate, monitor, and audit workflows and data flows at scale and with operational reliability.

With SLEDGEHammer, modern cloud-native applications can be deployed confidently and rapidly using hardened infrastructure with the required control implementation artifacts. A SLEDGEHammer platform can automatically generate OSCAL compatible evidence in support of a Continuous Authority to Operate (cATO) so that developers can confidently push validated code into production on an ongoing basis and mission owners and authorizing officials can approve and audit the applications with minimal staff and delays.

## What Is the Community Need?

The Primary Stakeholders are CNCF Open Source projects and CNCF Members (who may or may not have open source projects). These groups of volunteers and commercial entities want to increase the number of SLEDGEH enterprises and organizations utilizing CNCF member projects to the benefit of the larger community. New use cases, new real world applications, and increased security hardening and compliance assessment of CNCF projects benefits all current CNCF users.  

The secondary stakeholders are individual community participants from SLEDGEH organizations investigating the adoption and use of CNCF projects to help meet their mission goals. These architects, designers, operators and devops users require more than the extant documentation and general community guidance. They will benefit from actual real-world, hardened and tested implementation blueprints and specific compliance artifacts that will facilitate use of CNCF projects in highly regulated environments.

While many SLEDGEH organizations adopting Kubernetes in some way make minimal use of CI/CD to construct and deploy a containerized application, and generally embrace DevOps concepts to operate that application, the number of organizations that have successfully implemented “gitops'' and continuous security operations remains relatively small. By templating and hardening infrastructure and codifying security operations and compliance processes, it becomes realistic for more organizations to 10X the delivery of software and maintain continuous security and compliance. 

There are commercial entities providing consulting services and managed services for deep pocketed organizations. However, there is a gap in community adoption for less well-funded organizations, and/or those who may lack the in-house technical leadership and staff to build complex infrastructure de novo. There are also those who prefer to evolve from a trial hosted service into a more complex on-prem or hybrid Kubernetes-based infrastructure over time while learning organically instead of outsourcing infrastructure and operations permanently. 

Finally, regulators and the related community of internal SLEDGEH and external 3rd party compliance auditors and assessors are inadequately prepared to test and examine real world CNCF-based infrastructure. High velocity progress and change in CNCF projects is the norm, and assessors lack current and representative test environments, and lack real world compliance-as-code artifacts to review for their own assessment planning. This effort will help individual community members prepare for, and improve methodologies for, real world assessments required by regulatory frameworks and accreditation bodies. The better equipped auditors are for assessing compliance controls for CNCF-based infrastructure, the more quickly CNCF-based systems will be assessed and promoted to production use, increasing the impact CNCF has on large scale SLEDGEH cloud usage.

## Specifically How Do We Intend to Solve the Problems?

The CNCF projects in scope would provide deployable artifacts in the project repository for a NIST 800-53 rev 5 High compliant Kubernetes control plane, DevOps and SecOps infrastructure:

### Services In Scope

 1. Tenant isolated, multi-cluster capable, Kubernetes infrastructure for auto-scaling, High Security Control Baseline containerized workloads 
 2. Hardened deployment Infrastructure-as-Code and Platform Services, including GitOps CI/CD pipelines, security baseline scanning, developer self-service and provisioning, guard rails for compliance, and progressive delivery feature flag capabilities
 3. Hardened Container repository with hardened container image lifecycle management
 4. Supply chain security tooling, including security scanning
 5. Observability, Telemetry, Tracing, Logging and Monitoring infrastructure
 6. Compliance and configuration Policy-as-code and enforcement, and all necessary security policies, including admission control and drift detection
 7. Zero trust workloads that enforce cryptographic identity, encryption  in transit and at rest, behavior analysis, and security capability and compliance attestation; includes all compliant Cryptography and Key Management infrastructure, including key and secret storage support
 8. Hardened SDN and required network policies
 9. Continuous risk and vulnerability reporting, including Runtime signature and non-signature workload and network intrusion detection and prevention
 10. Hardened file and BLOB storage with high availability backup and restore  
 11. Developer toolchain, secure application packaging, debugging and break glass operations support 
 12. Hardened Ingress and API gateway support

Additional services that may be included based on community feedback and project participation:

-   Microservices infrastructure
    
-   ML services and infrastructure  

The following compliance and security workflows will be codified in devops tooling and/or CI/CD code, and included in the project open source artifacts:  

-   Support for Dry Run Compliance Assessment
    
-   Policy Generation and Management flows for C-R-U-D Cycles and Dependencies
    
-   Conditional Policy Enforcement and Policy Execution Ordering and Conflict Resolution
    
-   Policies for Protecting Sensitive Data
    
-   Day 2 Operations for Multi-Cluster hard-tenant isolation
    
-   Reporting Policy Violations
    
-   Policy Profiles: Inclusions and Exclusions with Labels, Namespaces and other Criteria
    
-   Managing Compliance Artifacts, References and Imported packages/artifacts
    
-   Examples of Remediation Playbook Automation
    
-   Reusable Library of Policy Artifacts and Rules
    
Will there be a hosted cloud test or production cloud as part of this effort?

It is the expectation that the artifacts developed will be deployed in a compliant, “authorized” public sector cloud environment, and that the hardened components and compliance artifacts will be sufficient to satisfy an independent 3rd party assessment for all NIST 800-54 rev 5 High Baseline controls. In addition SLEDGEHammer volunteer subject matter experts will be available to assist with an assessment, modeled after the recent Kubernetes External Audit effort led by Kubernetes sig-security.

Multiple cloud providers who maintain various public and private sector authorizations and certifications have expressed interest in hosting SLEDGEHammer. CNCF is not providing hosting services directly, although there may be funding or grants available to offset hosting fees for a lab environment and certification of an authorized system for use by CNCF members. 

While SLEDGEHammer artifacts will be deployable and operate with only open source components, optional commercial CNCF member features or services may be made available for SLEDGEH users to “opt-in” to. There may be additional hosting fees, or commercial licenses required for any SLEDGEH user.

SLEDGEH organizations who wish to deploy test and/or production clusters in a validated SLEDGEHammer hosted environment may be required to pay hosting fees, and collection of fees and contracting for services or licenses will be the sole responsibility of interested CNCF members or other entities who wish to provide commercial services to SLEDGEH buyers using the SLEDGEHammer open source artifacts.  

Neither CNCF, nor CNCF open source projects or members or individual volunteers are required to, or in any way expected to, pay any particular cloud provider, consultant, or service provider for participation in, or inclusion in, SLEDGEHammer - it is a purely volunteer, open effort. Use of CNCF member commercial tools or dependencies will be explicitly documented as optional. 

Commercial use and hosting of SLEDGEHammer artifacts must be managed by separate commercial entities who may or may not be affiliated with CNCF projects and member companies, but are in no way endorsed by CNCF, or any public or government entity. There is no operating agreement, Master Service Agreement, or other contractual agreement with CNCF.

## What is the Requirement for a CNCF Member to Participate?

### CNCF Open Source Projects

Any CNCF Sandbox, Incubating, or Graduated project may participate in, or be used by, SLEDGEHammer, regardless of contributor availability. However it is expected that all interested projects identify one primary and one secondary contributor point-of-contact. Participation in scheduled project informational sessions and updates, as well as lab testing sessions is highly encouraged, and subject matter expert support and resources for security hardening and compliance artifacts will be provided based on participation in these sessions.

The points-of-contact are asked to respond to, and with all best effort, complete tasks for:

-   Providing documentation and examples of project deployment modalities required for SLEDGEHammer
    
-   Provide new and existing test cases, analyze test results, and make recommendations for remediations of functional, performance, security or compliance issues identified
    
-   Provide contributor time to remediate and enhance the project to enable secure, compliant and reliable operation in the modalities supported by SLEDGEHammer
    
-   Participate in debug and diagnostic live test, assessment and audit sessions in a time zone reasonably convenient for contributors   

### CNCF Member Companies (Open Source and Commercial)

Any CNCF Member company or entity with both relevant CNCF open source code, and commercial offerings related to, or additive to CNCF projects in scope, may participate in SLEDGEHammer. However it is expected that these commercial entities identify one primary and one secondary contributor point-of-contact. Participation in scheduled project informational sessions and updates, as well as lab testing sessions is highly encouraged, and subject matter expert support and resources for security hardening and compliance artifacts will be provided based on participation in these sessions.

The points-of-contact are asked to respond to, and with all best effort, complete tasks for:

-   Providing documentation and examples of both open source and commercial project deployment modalities required for SLEDGEHammer
    
-   Provide new and existing open source and commercial test cases, analyze test results, and make recommendations for remediations of functional, performance, security or compliance issues identified
    
-   Provide contributor time to remediate and enhance both open source and commercial features to enable secure, compliant and reliable operation in the modalities supported by SLEDGEHammer
    
-   Participate in debug and diagnostic live test, assessment and audit sessions for both open source and commercial features in a time zone reasonably convenient for contributors

### CNCF Member Companies (No Open Source)

Any CNCF member in good standing may participate in SLEDGEHammer, regardless of open source code availability. These entities may have no code of relevance to offer, and merely wish to contribute time and expertise, or, they may have only commercial offerings that they wish to provide to users of SLEDGEHammer to augment or support core functionality, under a commercial license and/or Service Agreement. 

For either case, it is expected that all participating member organizations identify one primary and one secondary contributor point-of-contact. Participation in scheduled project informational sessions and updates, as well as lab testing sessions is highly encouraged, and subject matter expert support and resources for security hardening and compliance artifacts will be provided based on participation in these sessions.

### For Commercial Product Features

The points-of-contact for commercial entities with commercial features that are to be made available on SLEDGEHammer are required to respond to, and with all best effort, complete tasks for:

-   Providing documentation and examples of functionality/feature deployment modalities required for SLEDGEHammer
    
-   Provide new and existing test cases, analyze test results, and make recommendations for remediations of functional, performance, security or compliance issues identified
    
-   Provide contributor time to remediate and enhance the functionality/feature to enable secure, compliant and reliable operation in the modalities supported by SLEDGEHammer
    
-   Participate in debug and diagnostic live test, assessment and audit sessions for commercial functionality/features in a time zone reasonably convenient for contributors

### For Members without Products or Features In Scope
The points-of-contact for entities that not interested in offering functionality or features of any kind to SLEDGEHammer, and who only wish to participate in the process to learn more about compliance and security by assisting as subject matter experts or testers or other user advocates, are highly encouraged to:

-   Help document user stories and examples of functionality/feature requirements for SLEDGEHammer
    
-   Test and evaluate test results for SLEDGEHammer functionality and capabilities
    
-   Assist with compliance artifact creation, review, and processing
    
-   Act as scribes or assist with project communication
    
-   Act as user community advocates and write content for SLEDGEH user personas and entities to explain the features and functionality of SLEDGEHammer for increased adoption and feedback

### Individual CNCF Volunteer Participation and Code of Conduct

Any individual who wishes to participate in this effort is encouraged to communicate their interest by filing a Github Issue in the project repository. All participants - including CNCF member organization representatives and open source project participants, must agree to, and abide at all times with, the [current CNCF Code of Conduct](https://github.com/cncf/foundation/blob/main/code-of-conduct.md).

While all activities and artifacts are intended to be open and transparent to the community, specific CNCF project security embargo rules, as well as specific jurisdictional requirements (see below) may require limited distribution of some communications and test results until such time as the project security reviewers, and the CNCF Technical Oversight Committee, approves release.

### Participant Sovereignty and Regulatory Requirements

Given the locality of the initial member participants, and the need to coordinate meetings and group testing sessions, the primary focus of this 1.0 effort will be on United States compliance frameworks and requirements. As such, meetings and informational sessions, as well as testing sessions will be conducted in US working days and time zones. However, participation is open to all individuals and CNCF members as permitted by CNCF terms and rules, though specific project meetings, test sessions, and direct communications and test results may be subject to participating members’ national and jurisdictional restrictions on communications and or information sharing.

In no event will any proprietary, live production data of any kind be used for discovery, research, or testing, from any jurisdiction or location. Only publicly available and synthetic test data will be utilized for evaluation.

Cryptographic implementations and distribution of cryptographic technology may be subject to export control restrictions.

Subsequent sprints will expand the scope to include EU and APAC as and when community members in those regions and volunteer participants signal their interest and commitment levels. It is expected that commercial hosting partners that utilize SLEDGEHammer artifacts to provide authorized and audited services - including test labs - will impose limitations on access and collaboration, based on their jurisdictional compliance requirements.

### Anticipated Deliverables and Estimated Timelines

The primary deliverables include:

1.  A CNCF Sandbox Project and github repository
    
2.  All infrastructure as code artifacts necessary to deploy SLEDGEHammer in a cloud environment
    
3.  All policy as code artifacts necessary to assess a deployed SLEDGEHammer stack instance against NIST 800-53 rev 5 at the High Baseline level
    
4.  All compliance as code artifacts necessary to produce a System Security Plan, System Assessment Plan, System Assessment Report, and Plan of Actions and Milestones as well as supporting documentation, policy templates, and standard operating procedures templates mapped to the NIST 800-53 rev 5 High Baseline controls
    
5.  A US-based, cloud hosted assessment lab environment that has been audited by an accredited US-based 3rd Party Audit Organization, and which has a valid “Authority to Operate” for NIST 800-53 rev 5 High Baseline controls, such that any SLEDGEH enterprise (permitted to operate in the US) may use the SLEDGHammer services for pilot or small scale production usage in an authorized cloud environment.

The milestones and timeline anticipated:

-   Initial Kick Off Zoom Meeting for discussion of rules of the road - Jan 2023
    
-   Final adoption of rules of the project from member feedback; Sandbox Submission - Feb 2023
    
-   SME review and punch list creation for all participating projects and supporting components - March 2023
    
-   Completion of policy-as-code and OSCAL compliance-as-code artifacts - April 2023
    
-   Provisioning of Test and Assessment Lab Cloud Environment - May 2023
    
-   Completion of System Security Plan, System Assessment Plan - June 2023
    
-   Completion of independent 3rd party audit - July 2023
    
-   Authorization To Operate for SLEDGEH users - August 2023
    
Bi-weekly status Zoom meetings for participating members and volunteers will be held in alternating US Pacific and US Eastern time zones, and ad hoc as needed for specific milestones.

# Appendices

## CNCF Sandbox Application

[Please refer here for details](https://github.com/cncf/toc/blob/main/process/project_proposals.md). An issue will be created in the [Sandbox repo](https://github.com/cncf/sandbox).
