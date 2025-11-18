# FRIDGE Implementation Guide

**Version:** 1.0  
**Target Infrastructure:** UK AIRR (Dawn, Isambard-AI)  
**Compliance:** SATRE Specification, NHS DSP Toolkit

## 1. Overview

This guide provides a step-by-step approach to implementing the FRIDGE (Federated Research Infrastructure by Data Governance Extension) governance framework and operational processes. It is designed for organisations establishing FRIDGE for the first time.

## 2. Implementation Phases

### Phase 0: Safe Researcher Process (Prerequisite)
### Phase 1: Establish Governance Structure
### Phase 2: Implement Safe Setting Process
### Phase 3: Implement Safe Project Process
### Phase 4: Operationalise and Continuous Improvement

---

## Phase 0: Safe Researcher Process (Prerequisite)

**Objective:** Verify or establish Safe researcher approval and onboarding process

**Key Implementation Tasks:**
- Confirm attestation/agreement signing process in place and valid for governance extension
- Confirm suitable training in place
- Validate access provisioning workflows

**Critical Success Factors:**
- Process operational before Safe projects begin
- Clear approval criteria and delegation agreements (if applicable)

**Full Process Documentation:** [Safe Researcher Process](FRIDGE_Safe_Researcher_Process.md)

---

## Phase 1: Establish Governance Structure

**Objective:** Form the governance hierarchy and define organisational responsibilities

### Step 1.1: Identify and Engage Organisations

**Actions:**
1. Identify the four key organisations:
   - **Resource Allocator** - Organisation managing AIRR resource allocation
   - **FRIDGE Hosting Organisation** - Organisation providing AIRR infrastructure (Dawn/Isambard-AI)
   - **TRE Operator Organisation(s)** - Organisation(s) operating TREs
   - **Data Provider(s)** - Organisation(s) providing sensitive data

2. Engage senior leadership from each organisation
3. Secure commitment to participate in FRIDGE governance

**Outputs:**
- List of participating organisations
- Senior leadership commitment letters

---

### Step 1.2: Establish Top Management

**Actions:**
1. Identify Top Management representatives from participating organisations
2. Define the governance boundary scope
3. Document Top Management responsibilities and authority
4. Schedule initial Top Management meeting

**Key Decisions:**
- Governance boundary definition
- Strategic objectives for FRIDGE

**Outputs:**
- Top Management charter
- Governance boundary documentation

**Reference:** [Governing FRIDGE - Section 2.1](Governing_FRIDGE.md#21-top-management)

---

### Step 1.3: Form Operational Management Group

**Actions:**
1. Nominate representatives from each of the four organisations:
   - Resource Allocator representative
   - FRIDGE Hosting Organisation representative
   - TRE Operator Organisation representative
   - Data Provider / Information Governance representative

2. Define Operational Management Group:
   - Terms of reference
   - Decision-making authority
   - Escalation procedures


**Reference:** [Governing FRIDGE - Section 2.2](Governing_FRIDGE.md#22-operational-management-group)

---

### Step 1.4: Define Shared Responsibilities

**Actions:**
1. Review boundary accountability model
2. Document shared responsibilities for:
   - [Front Door TRE Boundary](FRIDGE_Governance_Extension_Architecture.md#23-front-door-tre-boundary)
   - [TRE Project Boundary](FRIDGE_Governance_Extension_Architecture.md#24-tre-project-boundary)
   - [FRIDGE TRE Hosting Boundary](FRIDGE_Governance_Extension_Architecture.md#25-fridge-tre-hosting-boundary)
   - [FRIDGE TRE Boundary](FRIDGE_Governance_Extension_Architecture.md#26-fridge-tre-boundary)

3. Create shared responsibility matrix
4. Obtain Top Management approval

**Outputs:**
- Shared responsibility matrix
- Boundary accountability documentation
- Approved governance framework

**Reference:** [FRIDGE Governance Extension Architecture - Boundaries](FRIDGE_Governance_Extension_Architecture.md#2-boundaries)

---

## Phase 2: Implement Safe Setting Process

**Objective:** Enable TRE Operators to obtain Safe Setting approval

**Overview:** The Safe Setting Process approves TRE Operators to host TREs on the FRIDGE platform. This one-time certification ensures the TRE deployment meets security and compliance requirements.

**Key Steps:**
1. TRE Operator submits Safe Setting request with deployment pattern and technical documentation
2. FRIDGE Hosting Organisation and Resource Allocator conduct initial review
3. TRE Operator deploys test environment with non-sensitive data
4. Independent audit and penetration testing conducted
5. FRIDGE Hosting Organisation and Resource Allocator grant Safe Setting approval

**Critical Success Factors:**
- Choose appropriate deployment pattern (Remote Job Submission or Full Stack TRE)
- Pass security audit and penetration testing
- Obtain dual approval from FRIDGE Hosting Organisation and Resource Allocator

**Full Process Documentation:** [Safe Setting Process](FRIDGE_Safe_Setting_Process.md)

---

## Phase 3: Implement Safe Project Process

**Objective:** Enable researchers to conduct Safe projects with sensitive data

**Prerequisites:** Safe Setting Process complete for TRE Operator

**Overview:** The Safe Project Process coordinates four organisations to establish and operate Safe projects. It includes parallel approval by Data Provider and Resource Allocator, followed by provisioning on both Front Door TRE and FRIDGE platform.

**Key Implementation Tasks:**
- Create project application templates and review criteria
- Establish parallel review process (Data Provider and Resource Allocator)
- Define provisioning procedures for all organisations
- Implement output review process

**Critical Success Factors:**
- Metadata sharing between Data Provider and Resource Allocator
- Clear Data Access Agreement template
- Efficient provisioning workflows
- Robust output review procedures

**Full Process Documentation:** [Safe Project Process](FRIDGE_SAFE_Project_Process.md)

---

## Phase 4: Operationalise and Continuous Improvement

**Objective:** Maintain and improve FRIDGE operations

**Ongoing**

**Overview:** Once FRIDGE is operational, establish monitoring systems, conduct regular reviews, and continuously improve processes based on lessons learned.

**Key Activities:**
- **Monitoring:** Each organisation monitors their area of responsibility (technical security, data access, resource utilisation, infrastructure security)
- **Regular Reviews:** Conduct compliance audits, governance framework reviews, and post-project retrospectives
- **Continuous Improvement:** Review feedback, propose improvements, obtain Operational Management Group approval, and update documentation

**References:**
- [Safe Project Process - Section 6](FRIDGE_SAFE_Project_Process.md#6-quality-assurance-and-compliance)
- [Governing FRIDGE - Section 7](Governing_FRIDGE.md#7-continuous-improvement)

---

## 3. Success Criteria

### Governance Structure
- [ ] Top Management established and meeting regularly
- [ ] Operational Management Group formed with representatives from all four organisations
- [ ] Shared responsibility matrix approved
- [ ] Escalation paths documented and communicated

### Safe Setting Process
- [ ] At least one TRE Operator has Safe Setting approval
- [ ] Test deployment successfully completed
- [ ] Audit and penetration testing passed
- [ ] Safe Setting certificate issued

### Safe Project Process
- [ ] Project application process operational
- [ ] Parallel review process functioning
- [ ] Provisioning procedures established
- [ ] At least one Safe project successfully provisioned

### Safe Researcher Process (Prerequisite)
- [ ] Researcher approval process operational
- [ ] Training programme in place
- [ ] Attestation process operational
- [ ] Access provisioning functioning
- [ ] Process reviewed against FRIDGE requirements

### Operations
- [ ] Monitoring systems operational
- [ ] Regular reporting established
- [ ] Review processes scheduled
- [ ] Continuous improvement cycle functioning

---

## 4. Key Resources

### Documentation
- [FRIDGE Governance Extension Architecture](FRIDGE_Governance_Extension_Architecture.md)
- [Governing FRIDGE](Governing_FRIDGE.md)
- [Safe Setting Process](FRIDGE_Safe_Setting_Process.md)
- [Safe Project Process](FRIDGE_SAFE_Project_Process.md)
- [Safe Researcher Process](FRIDGE_Safe_Researcher_Process.md)

### External References
- [SATRE Specification](https://satre-specification.readthedocs.io/en/stable/)
- [NHS DSP Toolkit](https://www.dsptoolkit.nhs.uk/)
- [AIRR Information](https://www.ukri.org/news/300-million-to-launch-first-phase-of-new-ai-research-resource/)

---


