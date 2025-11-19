# FRIDGE Governance Framework

**Federated Research Infrastructure by Data Governance Extension**

## Executive Summary

FRIDGE enables secure use of sensitive data for AI model development on large-scale supercomputers by extending Trusted Research Environment (TRE) governance onto the UK's AI Research Resource (AIRR). This repository provides a comprehensive governance framework and operational processes for implementing FRIDGE across AIRR supercomputing systems (Dawn at Cambridge and Isambard-AI at Bristol), with compatibility for public cloud platforms.

### Key Features

- **Federated Governance:** Coordinates four key organisations (Resource Allocator, FRIDGE Hosting Organisation, TRE Operator, Data Provider) under a unified governance structure
- **SATRE Compliant:** Meets the SATRE specification and NHS DSP Toolkit standards for secure data handling
- **Three Core Processes:** Safe Setting (TRE approval), Safe Project (project establishment), and Safe Researcher (researcher onboarding)
- **Clear Boundaries:** Defines accountability for governance, hosting, TRE, and project boundaries
- **Practical Implementation:** Step-by-step guide for establishing FRIDGE governance and processes

### Architecture Overview

FRIDGE extends TRE security from a "Front Door" TRE onto AIRR supercomputing facilities, enabling:
- Researchers to work within a Front Door TRE
- Remote job submission to FRIDGE compute resources
- Secure data access with strict information governance
- Isolated project spaces on shared AI infrastructure

## Documentation

### Core Documents

| Document | Description |
|----------|-------------|
| [FRIDGE Governance Extension Architecture](docs/FRIDGE_Governance_Extension_Architecture.md) | High-level architecture defining roles, boundaries, and responsibilities for the FRIDGE federation |
| [Governing FRIDGE](docs/Governing_FRIDGE.md) | Governance structure with Top Management and Operational Management Group, including escalation paths and decision-making authority |
| [FRIDGE Implementation Guide](docs/FRIDGE_Implementation_Guide.md) | Step-by-step guide for implementing FRIDGE governance and processes, from forming governance to operationalising all three Safe processes |

### Process Documents

| Process | Description | Frequency |
|---------|-------------|-----------|
| [Safe Setting Process](docs/FRIDGE_Safe_Setting_Process.md) | Approves TRE Operators to host TREs on FRIDGE platform through test deployment, audit, and penetration testing | Once per TRE Operator (or when deployment pattern changes) |
| [Safe Project Process](docs/FRIDGE_SAFE_Project_Process.md) | Establishes and operates Safe projects with parallel approval from Data Provider and Resource Allocator, followed by provisioning | Once per project |
| [Safe Researcher Process](docs/FRIDGE_Safe_Researcher_Process.md) | Approves and onboards Safe researchers through training, attestation, and access provisioning | Once per researcher |

## Key Organisations and Roles

FRIDGE coordinates four key organisations:

1. **Resource Allocator** - Manages AIRR resource allocation and ensures strategic alignment
2. **FRIDGE Hosting Organisation** - Provisions and secures resources on AIRR infrastructure (Dawn, Isambard-AI)
3. **TRE Operator Organisation** - Operates Front Door TRE and FRIDGE TRE with technical security controls
4. **Data Provider** - Approves data access and ensures all parties meet requirements

These organisations work together through:
- **Top Management** - Strategic oversight and governance boundary accountability
- **Operational Management Group** - Cross-organisational coordination and day-to-day operations

## Getting Started

### For Implementers

1. **Review Architecture:** Start with [FRIDGE Governance Extension Architecture](docs/FRIDGE_Governance_Extension_Architecture.md) to understand the overall structure
2. **Understand Governance:** Read [Governing FRIDGE](docs/Governing_FRIDGE.md) to understand the governance hierarchy
3. **Follow Implementation Guide:** Use [FRIDGE Implementation Guide](docs/FRIDGE_Implementation_Guide.md) for step-by-step implementation

### For TRE Operators

1. Complete [Safe Setting Process](docs/FRIDGE_Safe_Setting_Process.md) to obtain approval to host TREs on FRIDGE
2. Implement [Safe Project Process](docs/FRIDGE_SAFE_Project_Process.md) to enable project provisioning
3. Implement [Safe Researcher Process](docs/FRIDGE_Safe_Researcher_Process.md) to enable researcher onboarding

### For Researchers

1. Principal Investigators submit Safe project applications through the [Safe Project Process](docs/FRIDGE_SAFE_Project_Process.md)
2. Researchers complete training and attestation through the [Safe Researcher Process](docs/FRIDGE_Safe_Researcher_Process.md)
3. Access sensitive data within the TRE environment for AI model development

## Compliance and Standards

FRIDGE is designed to meet:
- **[SATRE Specification](https://satre-specification.readthedocs.io/en/stable/)** - Standard Architecture for Trusted Research Environments
- **[NHS DSP Toolkit](https://www.dsptoolkit.nhs.uk/)** - NHS Data Security and Protection Toolkit
- **ISO 27001** - Information security management (governance boundary may align with existing scope)

## Related Projects and Resources

### FRIDGE Project
- **Funding:** UK Research and Innovation (UKRI)
- **Partners:** University College London (UCL), University of Cambridge, University of Bristol, The Alan Turing Institute
- **Infrastructure:** UK AI Research Resource (AIRR)

### AIRR Supercomputing Systems
- **Dawn** - University of Cambridge supercomputing facility
- **Isambard-AI** - University of Bristol supercomputing facility

### Related Initiatives
- **[SATRE Specification](https://satre-specification.readthedocs.io/en/stable/)** - Developed by DARE UK Phase 1 Driver Projects
- **[TREvolution](https://www.hdruk.ac.uk/infrastructure/trevolution/)** - Enhancing TRE capabilities
- **[DARE UK](https://dareuk.org.uk/)** - Data and Analytics Research Environments UK

## About This Repository

### Author and Affiliation

**Author:** Tim Machin  
**Organisation:** Advanced Research Computing, University College London (UCL)  
**Project:** FRIDGE - Federated Research Infrastructure by Data Governance Extension

### Purpose

This repository documents the governance framework and operational processes for FRIDGE, enabling secure use of sensitive data on AI supercomputing infrastructure. The framework is designed to be:
- **Reusable:** Applicable to other TRE operators and supercomputing facilities
- **Standards-compliant:** Meets SATRE and NHS requirements
- **Practical:** Provides actionable guidance for implementation

### Development Tooling

This documentation was developed using:
- **AI Assistant:** Kiro IDE
- **Model:** Claude 3.7 Sonnet (Anthropic)
- **Development Approach:** Iterative prompt-based documentation generation with human oversight and editing and domain expertise

All prompts used during development are documented in [sourcefiles/prompts_log.md](sourcefiles/prompts_log.md) to provide transparency about the documentation creation process.

## Contact and Support

For more information about FRIDGE:
- **Advanced Research Computing - UCL – University College London:** [https://www.ucl.ac.uk/advanced-research-computing](https://www.ucl.ac.uk/advanced-research-computing)
- **AIRR Information:** [https://www.ukri.org/what-we-do/creating-world-class-research-and-innovation-infrastructure/digital-research-infrastructure/ai-research-resource/](https://www.ukri.org/what-we-do/creating-world-class-research-and-innovation-infrastructure/digital-research-infrastructure/ai-research-resource/)

---

**Version:** 1.0  
**Last Updated:** November 2025  
**Target Infrastructure:** UK AIRR (Dawn, Isambard-AI)  
**Compliance:** SATRE Specification, NHS DSP Toolkit
