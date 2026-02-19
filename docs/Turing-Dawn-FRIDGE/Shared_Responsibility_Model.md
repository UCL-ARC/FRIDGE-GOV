# Shared Responsibility Model: Turing-Dawn-FRIDGE

**TRE Operator Organisation:** The Alan Turing Institute  
**FRIDGE Hosting Organisation:** Cambridge Open Zettascale Lab  
**FRIDGE Instance:** Turing-Dawn-FRIDGE  
**Version:** 1.0  
**Compliance:** SATRE Specification, NHS DSP Toolkit

## 1. Overview

This document defines the shared responsibility model between The Alan Turing Institute (TRE Operator Organisation) and Cambridge Open Zettascale Lab (FRIDGE Hosting Organisation) for the Turing-Dawn-FRIDGE instance. This model follows the approach used by major cloud providers (AWS, Azure, GCP) where responsibilities are clearly delineated between the infrastructure provider and the customer.

### 1.1 Key Principle

**The Alan Turing Institute retains full accountability for the security of the Turing-Dawn-FRIDGE infrastructure and all user data.** Cambridge Open Zettascale Lab is accountable for the security of the Dawn supercomputer. Where processes, applications, data or infrastructure are shared responsibilities are defined in more detail.

### 1.2 Shared Responsibility Diagram

```mermaid
graph TB
    subgraph Turing["Alan Turing Institute (TRE Operator)"]
        TuringResp["<b>Turing Responsibilities</b><br/>• FRIDGE TRE Security<br/>• Front Door TRE Security<br/>• Data Security & Encryption<br/>• Access Control & Identity<br/>• Applications & Workloads<br/>• Project Boundaries<br/>• Researcher Approval<br/>• Output Review"]
    end
    
    subgraph Shared["Shared Responsibilities"]
        SharedResp["<b>Joint Accountability</b><br/>• Network Isolation<br/>• Resource Allocation<br/>• Incident Response Coordination<br/>• Change Management"]
    end
    
    subgraph Cambridge["Cambridge Open Zettascale Lab (FRIDGE Hosting)"]
        CambridgeResp["<b>Cambridge Responsibilities</b><br/>• Dawn Infrastructure Security<br/>• Physical Security<br/>• Hardware & Facilities<br/>• Network Infrastructure<br/>• Platform Services<br/>• Capacity Management"]
    end
    
    TuringResp -.->|Defines Requirements| SharedResp
    CambridgeResp -.->|Implements Controls| SharedResp
    
    style Turing fill:#e6f3ff
    style Shared fill:#fff4e6
    style Cambridge fill:#f0e6ff
```

## 2. Responsibility Matrix

### 2.1 Alan Turing Institute Responsibilities

The Alan Turing Institute, as TRE Operator Organisation, is accountable for:

| Area | Specific Responsibilities | DSPT Ref  | Reference |
|------|--------------------------|-----------|------------|
| **FRIDGE TRE Security** | • Deploy and configure FRIDGE TRE<br/>• Implement technical security controls<br/>• Manage TRE software and updates<br/>• Configure job processing systems<br/>• Maintain SATRE compliance | • 8.1.4, 8.3.5, 8.4.1, 9.5.3 <br/> • 8.4.1, 8.4.2, 9.1.1, 9.6.1, 9.4.4 <br/> • 8.1.4, 8.2.1, 8.3.2, 8.3.5, 8.4.2, 9.2.1, 9.2.3 <br/> • 9.5.3, 9.5.1, 8.4.1, 8.4.2, 9.1.1, 9.6.1 <br/> • 4.5.3, 4.4.1, 8.4.1, 8.3.5, 9.2.1, 7.1.2, 7.3.1, 10.2.1 | [FRIDGE TRE Boundary](../FRIDGE_Governance_Extension_Architecture.md#36-fridge-tre-boundary) |
| **Front Door TRE Security** | • Operate Front Door TRE<br/>• Implement infrastructure management<br/>• Manage study/project processes<br/>• Maintain TRE capabilities | • 4.2.4, 4.3.1, 4.5.3, 9.6.1, 9.1.1, 8.4.1 <br/> • 8.4.1, 8.4.2, 9.5.1, 9.5.3, 9.1.1, 9.6.1 <br/> • 1.3.7, 1.3.8, 4.1.1, 4.2.4, 6.1.1 <br/> • 4.5.3, 4.4.1, 8.1.4, 8.3.5, 8.4.1, 9.6.1, 10.2.1 | [Front Door TRE Boundary](../FRIDGE_Governance_Extension_Architecture.md#33-front-door-tre-boundary) |
| **Data Security** | • Encrypt data at rest and in transit<br/>• Manage encryption keys<br/>• Control data lifecycle<br/>• Implement data handling policies<br/>• Ensure data isolation between projects | • 9.3.6, 9.5.2, 8.4.1 <br/> • 4.3.1, 4.4.1, 8.3.5, 8.4.1, 9.3.6 <br/> • 1.4.1, 1.4.3, 1.3.7, 1.1.2 <br/> • 1.3.1, 1.3.7, 1.3.8, 1.4.1, 1.4.3  <br/> • 44.1.1, 4.2.4, 9.6.1, 9.5.3, 8.4.1, 1.3.7 |[TRE Project Boundary](../FRIDGE_Governance_Extension_Architecture.md#34-tre-project-boundary) |
| **Access Control & Identity** | • Manage user accounts and authentication<br/>• Implement role-based access control<br/>• Provision researcher access<br/>• Verify approvals before access<br/>• Manage credentials and tokens | • 4.1.1, 4.2.4, 4.5.3, 4.5.4, 4.3.1, 4.4.1 <br/> • 4.1.1, 4.2.4, 4.3.1, 4.5.3, 1.3.7 <br/> • 4.1.1, 4.2.4, 4.5.3, 4.3.1, 1.3.7 <br/> • 4.1.1, 4.2.4, 4.3.1, 4.4.1, 1.3.7 <br/> • 4.5.3, 4.5.4, 4.3.1, 4.4.1, 9.5.1, 8.3.5 | [Safe Researcher Process](../FRIDGE_Safe_Researcher_Process.md) |
| **Applications & Workloads** | • Deploy and manage applications<br/>• Configure job submission systems<br/>• Implement output review processes<br/>• Manage software dependencies | • 9.5.1, 9.5.3, 8.3.5, 8.1.4, 9.2.1, 9.4.4 <br/> • 9.5.3, 9.5.1, 8.4.1, 8.4.2, 9.1.1, 9.6.1 <br/> • 8.1.4, 8.2.1, 8.3.5, 9.5.3, 9.5.1, 9.4.4 <br/> • 1.3.7, 1.1.2, 4.4.1, 6.1.1, 9.3.6, 10.2.2 | [Safe Project Process](../FRIDGE_SAFE_Project_Process.md) |
| **Project Boundaries** | • Establish project workspaces<br/>• Implement project isolation<br/>• Manage project lifecycle<br/>• Coordinate with Data Providers | • 1.3.7, 1.3.8, 4.1.1, 9.5.3, 9.6.1, 8.4.1 <br/> • 4.1.1, 4.2.4, 9.5.1, 9.6.1, 9.3.5, 1.3.7 <br/> • 1.1.2, 1.3.7, 4.2.4, 4.4.1, 9.5.3, 1.4.1, 1.4.3 <br/> • 1.1.2, 10.1.2, 10.2.2, 10.2.5, 1.2.4, 9.3.6 | [TRE Project Boundary](../FRIDGE_Governance_Extension_Architecture.md#34-tre-project-boundary) |
| **Governance & Compliance** | • Maintain SATRE compliance<br/>• Implement information governance<br/>• Conduct output reviews<br/>• Manage researcher training<br/>• Maintain audit trails | • 4.5.3, 4.4.1, 8.4.1, 8.3.5, 9.2.1, 7.1.2, 10.2.1 <br/> • 1.1.2, 1.1.5, 1.3.1, 1.3.2, 1.3.6, 1.4.1, 6.1.1, 10.2.2 <br/> • 2.1.1, 3.1.1, 3.2.1, 3.3.1, 3.4.1 <br/> • 1.3.7, 1.1.2, 4.4.1, 6.1.1, 9.3.6, 10.2.2 <br/> • 4.4.1, 4.3.3, 6.1.1, 6.3.5, 9.5.3, 9.6.1, 1.4.3, 10.2.2 | [Governing FRIDGE](../Governing_FRIDGE.md) |

[DSPT Controls reference file]("./Images/DSPT controls.xlsx")

### 2.2 Cambridge Open Zettascale Lab Responsibilities

Cambridge Open Zettascale Lab, as FRIDGE Hosting Organisation, is accountable for:

| Area | Specific Responsibilities | DSPT Ref | Reference |
|------|--------------------------|----------|-----------|
| **Dawn Infrastructure Security** | • Secure Dawn supercomputer platform<br/>• Maintain platform security controls<br/>• Monitor infrastructure security<br/>• Implement platform hardening<br/>• Manage platform vulnerabilities | • 8.4.1, 8.4.2, 8.3.5 <br/> • 9.5.1, 8.1.4, 9.4.4 <br/> • 6.1.1, 6.3.1, 6.3.5 <br/> • 8.4.1, 9.1.1, 9.6.1 <br/> • 8.4.3, 9.2.1, 9.2.3, 9.4.4 | [FRIDGE TRE Hosting Boundary](../FRIDGE_Governance_Extension_Architecture.md#35-fridge-tre-hosting-boundary) |
| **Physical Security** | • Secure data centre facilities<br/>• Control physical access<br/>• Maintain environmental controls<br/>• Implement physical monitoring<br/>• Manage facility incidents | • 1.3.13 <br/> • 1.3.13 <br/> • 7.1.1 <br/> • 1.3.13 <br/> • 6.1.1, 6.1.2 | [FRIDGE TRE Hosting Boundary](../FRIDGE_Governance_Extension_Architecture.md#35-fridge-tre-hosting-boundary) |
| **Hardware & Facilities** | • Maintain compute hardware<br/>• Manage storage systems<br/>• Ensure hardware reliability<br/>• Implement hardware lifecycle<br/>• Manage hardware failures | • 8.1.4, 8.4.2 <br/> • 7.3.1, 7.3.4 <br/> • 7.1.1, 7.2.1 <br/> • 1.4.3 <br/> • 7.1.2, 7.2.1 | [FRIDGE TRE Hosting Boundary](../FRIDGE_Governance_Extension_Architecture.md#35-fridge-tre-hosting-boundary) |
| **Network Infrastructure** | • Provide network connectivity<br/>• Maintain network hardware<br/>• Implement base network security<br/>• Monitor network performance<br/>• Manage network incidents | • 9.1.1, 9.6.1 <br/> • 9.1.1, 8.4.2 <br/> • 9.6.1, 9.3.5 <br/> • 6.3.1 <br/> • 6.1.1, 6.1.2 | [FRIDGE TRE Hosting Boundary](../FRIDGE_Governance_Extension_Architecture.md#35-fridge-tre-hosting-boundary) |
| **Platform Services** | • Operate Dawn platform services<br/>• Maintain service availability<br/>• Implement platform monitoring<br/>• Manage platform updates<br/>• Provide platform support | • 8.4.1, 8.3.5 <br/> • 7.1.1, 7.1.2 <br/> • 6.1.1, 6.3.5 <br/> • 8.3.5, 8.1.4, 9.4.4 <br/> • 10.1.2, 10.2.1 | [FRIDGE TRE Hosting Boundary](../FRIDGE_Governance_Extension_Architecture.md#35-fridge-tre-hosting-boundary) |
| **Capacity Management** | • Manage compute capacity<br/>• Monitor resource utilisation<br/>• Plan capacity expansion<br/>• Allocate resources per agreements<br/>• Report on capacity | • 7.1.1 <br/> • 6.3.5 <br/> • 7.1.1, 7.2.1 <br/> • 4.1.1, 4.2.4 <br/> • 7.1.1, 5.2.1 | [Safe Project Process](../FRIDGE_SAFE_Project_Process.md) |

### 2.3 Shared Responsibilities

The following responsibilities require coordination and joint accountability between both organisations:

| Area | Turing Responsibilities | Cambridge Responsibilities | Coordination Mechanism |
|------|------------------------|---------------------------|------------------------|
| **Network Isolation** | • Define network isolation requirements<br/>• Specify security policies<br/>• Configure TRE network controls<br/>• Monitor TRE network traffic | • Implement network segmentation<br/>• Configure platform network policies<br/>• Enforce isolation at infrastructure level<br/>• Monitor platform network security | Operational Management Group reviews network architecture and approves changes |
| **Resource Allocation** | • Define resource requirements<br/>• Request resource allocation<br/>• Monitor resource usage<br/>• Manage project resources | • Provision allocated resources<br/>• Implement resource quotas<br/>• Monitor platform capacity<br/>• Report resource availability | Resource Allocator coordinates allocation decisions with both parties |
| **Incident Response** | • Detect and respond to TRE incidents<br/>• Investigate security events<br/>• Implement remediation<br/>• Report incidents per agreements | • Detect and respond to platform incidents<br/>• Investigate infrastructure events<br/>• Implement platform remediation<br/>• Report incidents per agreements | Joint incident response procedures with defined escalation paths |
| **Change Management** | • Plan TRE changes<br/>• Assess change impact<br/>• Implement TRE changes<br/>• Validate TRE functionality | • Plan platform changes<br/>• Assess platform impact<br/>• Implement platform changes<br/>• Communicate platform changes | Operational Management Group coordinates changes affecting both parties |

## 3. Boundary Accountability

### 3.1 Governance Boundary

**Accountable:** Top Management (joint oversight from both organisations)

**Scope:** The governance boundary encompasses the entire Turing-Dawn-FRIDGE system including Front Door TRE, FRIDGE TRE on Dawn, and all interconnected systems.

