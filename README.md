# NIST CSF 2.0 Gap Assessment

## Executive Summary

This assessment evaluated the organization’s current cybersecurity posture using the NIST Cybersecurity Framework (CSF) 2.0. The objective was to identify gaps in governance, risk management, and technical controls, and to develop a prioritized roadmap to improve cybersecurity maturity.

Overall, the organization’s cybersecurity maturity aligns with **NIST CSF Tier 1: Partial**. While several security tools and practices are in place, they are inconsistently implemented and lack formal governance, risk-based prioritization, and executive oversight.

<img src="csf-functions.jpg" width="500">

### Key Findings
- Cybersecurity governance and executive oversight are not formally established
- Asset, data, and risk visibility are incomplete, limiting effective prioritization
- Preventive security controls exist but are inconsistently enforced
- Detection, response, and recovery capabilities are largely informal or undocumented
- Third-party cybersecurity risk is unmanaged

### Top Cybersecurity Risks
- Increased likelihood of account compromise due to inconsistent MFA enforcement
- Delayed detection of security incidents due to lack of centralized monitoring
- Extended recovery time due to absence of formal incident response and recovery processes
- Exposure to third-party risk without standardized vendor assessments
- Inability to prioritize remediation efforts due to undefined risk tolerance

### Recommended Path Forward
The organization should prioritize establishing foundational governance and risk management capabilities and target progression to **NIST CSF Tier 2: Risk-Informed**. This includes defining cybersecurity ownership, formalizing risk assessment processes, enforcing baseline security controls, and improving visibility through centralized monitoring.

A phased improvement roadmap has been developed to guide this progression while balancing security improvements with operational practicality.

## Company Profile

**Organization Type:** B2B SaaS company  
**Employee Count:** Approximately 100  
**Industry:** Cloud-native software services  
**Customer Base:** Small to mid-sized businesses  
**Regulatory Exposure:** Moderate  

The organization processes customer data and relies heavily on service availability to meet contractual and operational obligations. While not operating in a highly regulated industry, the company must maintain reasonable controls to ensure confidentiality, integrity, and availability of systems and data.

### Technology Environment

- **Identity and Email:** Microsoft 365 or Google Workspace
- **Cloud Provider:** Microsoft Azure
- **Endpoint Operating System:** Windows laptops
- **Endpoint Security:** Microsoft Defender for Endpoint
- **Password Management:** LastPass
- **Architecture:** SaaS-first with minimal on-premises infrastructure

## Assessment Objective

The purpose of this assessment is to evaluate the organization’s current cybersecurity posture using the NIST Cybersecurity Framework 2.0, identify gaps across governance, risk management, and technical controls, and develop a prioritized roadmap to improve cyber risk management maturity.

## Scope and Assumptions

### In Scope
- Corporate IT environment
- Cloud infrastructure hosted in Microsoft Azure
- SaaS applications supporting core business functions
- End-user endpoints
- Identity and access management
- Third-party SaaS vendors

### Out of Scope
- Secure software development lifecycle
- Application penetration testing
- Customer-managed environments

### Key Assumptions
- No formal cybersecurity governance program exists
- Cybersecurity responsibilities are primarily handled by IT operations
- Existing security tooling is inconsistently used
## Current Cybersecurity Posture Summary

The following summary reflects the organization’s current cybersecurity capabilities based on interviews, documentation review, and high-level technical observations.

### Governance

- No formally documented cybersecurity strategy approved by executive leadership
- Cybersecurity responsibilities embedded within IT operations
- No defined executive or board-level oversight of cybersecurity risk

### Asset Management

- Endpoints are deployed using standardized corporate images
- Asset inventory exists but does not include ownership or business criticality
- Cloud resources are tracked at a high level but not risk-ranked

### Identity and Access Management

- Centralized identity management using Entra ID (Azure AD)
- Multi-factor authentication enforced for some users, not universally
- No privileged access management solution in place
- Access is granted through ticket-based requests
- Periodic access reviews are informal or ad hoc

### Vulnerability Management

- Microsoft Defender provides vulnerability visibility
- No documented vulnerability management policy
- Vulnerability remediation is reactive and inconsistently prioritized
- No defined service-level objectives for patching

### Logging and Monitoring

- Endpoint alerts monitored through Microsoft Defender
- No centralized security information and event management solution
- Limited visibility into cloud and SaaS activity logs

### Incident Response

- No formal incident response plan
- Incidents are handled reactively by IT staff
- No incident tabletop exercises or post-incident reviews

### Third-Party Risk Management

- Extensive use of third-party SaaS vendors
- No formal third-party risk management process
- Vendor security reviews are not standardized or documented

## NIST CSF 2.0 Gap Assessment Results

The NIST Cybersecurity Framework 2.0 was used as a structured lens to evaluate the organization’s cybersecurity capabilities across six core functions.

<details > 
<summary> <h3> See Results</h3> </summary>

### ![Screenshot 2024-10-28 134244](https://github.com/user-attachments/assets/c536c78f-b8d2-4988-a1ad-ea1b0222bd41)
**Assessment Result:** Largely Not Implemented 

| Capability | Current State | Evidence Reviewed | Gap Identified | Recommendation |
|-----------|---------------|------------------|----------------|----------------|
| Cybersecurity strategy | Not implemented | No documented strategy or executive-approved roadmap | Lack of strategic direction and prioritization | Develop and approve a cybersecurity strategy aligned to business objectives |
| Executive oversight | Not implemented | No governance committee or reporting cadence | Cyber risk not visible to leadership | Establish executive-level cybersecurity oversight and reporting |
| Risk appetite definition | Not implemented | No documented risk tolerance statements | Inability to prioritize risk consistently | Define and document organizational cyber risk tolerance |
| Roles and responsibilities | Partially implemented | Informal IT ownership, no RACI | Accountability gaps across functions | Define and document cybersecurity roles and responsibilities |

### ![Screenshot 2024-10-28 134430](https://github.com/user-attachments/assets/bd218bc5-9048-4d91-96fd-77aba367d87b)
**Assessment Result:** Partially Implemented

| Capability | Current State | Evidence Reviewed | Gap Identified | Recommendation |
|-----------|---------------|------------------|----------------|----------------|
| Asset inventory | Partially implemented | Endpoint inventory exists without ownership or criticality | Assets cannot be prioritized by business impact | Implement asset inventory with ownership and criticality classification |
| Data classification | Not implemented | No data classification or labeling scheme | Sensitive data cannot be protected appropriately | Establish and implement data classification standards |
| Business criticality | Not implemented | No documented critical systems or services | Inability to prioritize recovery and protection efforts | Identify and document business-critical systems and services |
| Risk assessment | Not implemented | No formal cyber risk assessments conducted | Risks are not consistently identified or prioritized | Establish a formal cybersecurity risk assessment process |
| Third-party dependencies | Not implemented | Vendor list exists without risk context | Third-party risks are unmanaged | Identify and classify third-party dependencies by risk |

### ![Screenshot 2024-10-28 134438](https://github.com/user-attachments/assets/f6554061-0d01-49e9-91df-b102eb4b8ac7)
**Assessment Result:** Partially Implemented

| Capability | Current State | Evidence Reviewed | Gap Identified | Recommendation |
|-----------|---------------|------------------|----------------|----------------|
| Identity and access protections | Partially implemented | MFA enforced for some users; access granted via tickets | Inconsistent MFA enforcement and access reviews | Enforce MFA for all users and establish periodic access reviews |
| Privileged access management | Not implemented | No dedicated privileged access controls | Elevated privileges are unmanaged | Implement privileged access management controls |
| Vulnerability remediation | Partially implemented | Defender vulnerability data reviewed inconsistently | Vulnerabilities are not remediated based on risk | Establish a formal vulnerability management and remediation process |
| Data protection controls | Partially implemented | Data stored in Azure without classification or DLP | Sensitive data is not consistently protected | Implement data classification and data loss prevention controls |
| Secure configuration management | Partially implemented | Standard images used without formal change control | Configuration changes are not consistently governed | Establish configuration and change management processes |

### ![Screenshot 2024-10-28 134447](https://github.com/user-attachments/assets/26e591c9-9ee6-454f-9f5b-37062bec1d0c)
**Assessment Result:** Not Implemented


| Capability | Current State | Evidence Reviewed | Gap Identified | Recommendation |
|-----------|---------------|------------------|----------------|----------------|
| Centralized logging | Not implemented | Logs stored locally across systems | Security events are fragmented and difficult to correlate | Implement centralized log collection across endpoints, cloud, and SaaS services |
| Security event monitoring | Not implemented | No continuous monitoring or alert triage process | Potential threats may go unnoticed | Establish continuous security monitoring and alert review procedures |
| Anomaly detection | Not implemented | No defined baselines for normal activity | Abnormal behavior cannot be reliably identified | Define behavioral baselines and implement anomaly detection use cases |
| Alert escalation procedures | Not implemented | No documented escalation thresholds or workflows | Delayed or inconsistent incident response | Define alert severity levels and escalation procedures |
| Detection roles and responsibilities | Partially implemented | IT staff respond to alerts informally | No clear ownership for detection activities | Define and document detection and monitoring responsibilities |

### ![Screenshot 2024-10-28 134456](https://github.com/user-attachments/assets/bfdf2e21-ced1-4767-8ac6-4ec982b6f5e3)
**Assessment Result:** Not Implemented

| Capability | Current State | Evidence Reviewed | Gap Identified | Recommendation |
|-----------|---------------|------------------|----------------|----------------|
| Incident response planning | Not implemented | No documented incident response plan | Organization lacks a defined approach to handling incidents | Develop and approve a formal incident response plan |
| Incident roles and responsibilities | Not implemented | No documented incident response roles or on-call ownership | Response efforts would be uncoordinated during an incident | Define incident response roles and responsibilities |
| Incident escalation procedures | Not implemented | No documented escalation thresholds or workflows | Delays and confusion during high-severity incidents | Establish incident severity levels and escalation procedures |
| Incident communications | Partially implemented | Ad hoc internal communications during incidents | Inconsistent stakeholder communication | Define internal and external incident communication procedures |
| Incident analysis and documentation | Not implemented | No formal incident tracking or post-incident reviews | Lessons learned are not captured or applied | Implement incident documentation and post-incident review process |

### ![Screenshot 2024-10-28 134503](https://github.com/user-attachments/assets/10ef5d64-da8b-41df-a0fe-56acb244fd1c)
**Assessment Result:** Partially Implemented


| Capability | Current State | Evidence Reviewed | Gap Identified | Recommendation |
|-----------|---------------|------------------|----------------|----------------|
| Recovery planning | Partially implemented | IT disaster recovery procedures exist without cyber-specific recovery focus | Cyber incidents may not be fully accounted for in recovery efforts | Develop recovery procedures aligned to cybersecurity incidents |
| Backup and restoration | Partially implemented | Backups are performed but not consistently tested for cyber scenarios | Uncertainty around restoration effectiveness after incidents | Establish regular backup testing and validation processes |
| Recovery communications | Not implemented | No defined recovery communication procedures | Stakeholders may lack clarity during recovery phase | Define internal and external recovery communication plans |
| Lessons learned integration | Not implemented | No formal post-incident improvement process | Recovery efforts do not improve future resilience | Implement a lessons learned and continuous improvement process |
</details > 

## Key Cybersecurity Risks

- Inconsistent MFA enforcement increases the likelihood of account compromise
- Lack of centralized logging limits the organization’s ability to detect and investigate security events
- Absence of a formal incident response plan increases operational and recovery risk
- Unmanaged third-party risk exposes customer data and service availability
- Undefined vulnerability remediation timelines increase exposure to known exploits

## CSF Tier Assessment

<img src="csf-tiers.jpg" width="600">

Based on the findings of this assessment, the organization’s current cybersecurity maturity aligns with **NIST CSF Tier 1: Partial**.

At this tier, cybersecurity risk management activities are largely reactive, inconsistently implemented, and primarily driven by operational IT needs rather than formal governance or risk-based decision making. While some security controls and tools are in place, they are not consistently governed, measured, or aligned to defined risk tolerance.

### Current Tier: Tier 1 – Partial

Characteristics observed:
- Cybersecurity governance is informal and lacks executive oversight
- Risk management processes are not formally established
- Security activities are reactive rather than proactive
- Policies, procedures, and roles are incomplete or undocumented

### Target Tier: Tier 2 – Risk-Informed

The recommended target state for the organization is **NIST CSF Tier 2: Risk-Informed**.

At this tier, cybersecurity risk management practices are formally established, leadership is aware of cybersecurity risks, and risk-based prioritization begins to inform decision making. This target tier represents a realistic and achievable maturity improvement for a mid-sized SaaS organization without overextending resources or creating unnecessary operational burden.

Target Tier 2 objectives include:
- Defined cybersecurity governance and ownership
- Documented risk assessment and risk management processes
- Consistent application of baseline security controls
- Leadership visibility into cybersecurity risk and priorities

A longer-term progression toward **Tier 3: Repeatable** may be considered after Tier 2 capabilities are established and operating effectively.


## Improvement Roadmap

### Phase 1: Foundation (0–90 Days)
- Establish cybersecurity governance and ownership
- Enforce MFA for all users
- Define a vulnerability management process
- Draft core cybersecurity policies

### Phase 2: Maturity (3–6 Months)
- Implement centralized logging and monitoring
- Formalize incident response procedures
- Conduct access reviews
- Introduce third-party risk assessments

### Phase 3: Optimization (6–12 Months)
- Mature detection and response capabilities
- Perform incident response tabletop exercises
- Align key controls to NIST 800-53
- Establish continuous risk monitoring

## Appendix: Evidence Request Checklist

The following evidence would typically be reviewed to validate assessment findings:
- Cybersecurity policies and standards
- Risk assessment and risk register documentation
- Asset and data inventories
- Access control and MFA configurations
- Vulnerability management reports
- Logging and monitoring dashboards
- Incident response and recovery documentation
- Third-party vendor security assessments
