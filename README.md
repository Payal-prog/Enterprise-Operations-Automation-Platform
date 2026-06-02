# Enterprise Operations Automation Platform

## Overview

Designed and developed an internal enterprise automation platform using **C# WinForms**, **PowerShell**, **Hyper-V**, and **Linux SSH automation** to streamline infrastructure provisioning, environment configuration, diagnostics, and operational support workflows.

The platform consolidated dozens of repetitive support and infrastructure tasks into a centralized graphical interface, reducing manual effort, improving consistency, and accelerating troubleshooting across Windows and Linux environments.

---

## Key Business Impact

### Infrastructure Provisioning Automation

Automated end-to-end Hyper-V environment creation including:

* Hyper-V enablement and validation
* Virtual switch creation
* VPN adapter provisioning
* Generation 2 VM deployment
* Virtual disk attachment
* Secure Boot configuration
* CPU and memory allocation
* Boot order automation

Reduced virtual machine provisioning from a multi-step manual process to a single-click workflow.

---

### Environment Validation & Health Monitoring

Implemented continuous system validation modules that automatically:

* Monitor VPN connectivity
* Detect assigned VPN addresses
* Retrieve system IP information
* Validate Hyper-V configuration
* Identify hardware specifications
* Parse application hardware configurations
* Detect printer and peripheral mappings
* Validate workstation readiness

Background monitoring threads continuously refresh system state and infrastructure status.

---

### Linux Operations & Remote Diagnostics

Integrated SSH-based automation to interact with enterprise Linux environments.

Capabilities include:

* Remote log collection
* Deployment diagnostics
* Server health validation
* Real-time log monitoring
* SSH command execution
* Log archival and retrieval
* Cross-platform troubleshooting

Engineers can instantly access deployment and application logs without manually connecting to remote systems.

---

### Configuration Management

Implemented automation modules for:

* Firewall rule validation
* Firewall rule deployment
* Registry-based configuration updates
* Hardware configuration management
* Environment-specific application settings
* Network parameter configuration
* Terminal provisioning

---

### Operational Automation

Automated numerous repetitive operational activities including:

* Computer renaming
* User logoff and restart actions
* Application updates
* VPN configuration
* Hardware validation
* Environment setup
* Server configuration management

---

## Architecture

```text
+------------------------------------------------+
|              C# WinForms Dashboard             |
+------------------------------------------------+
                     |
     +---------------+---------------+
     |                               |
     v                               v

PowerShell Engine                SSH Engine
(System.Management.Automation)   (SSH.NET)

     |                               |
     v                               v

Windows Infrastructure       Linux Infrastructure

- Hyper-V                    - Application Servers
- Virtual Switches           - Deployment Logs
- VPN Adapters               - Runtime Diagnostics
- Registry                   - Remote Commands
- Firewall Rules             - Monitoring
```

## Technology Stack

### Programming

* C#
* .NET Framework
* PowerShell

### Infrastructure & Virtualization

* Hyper-V
* Virtual Switches
* VPN Adapters
* Windows Registry
* WMI

### Linux Administration

* SSH
* SFTP
* Remote Diagnostics

### Libraries

* SSH.NET
* Newtonsoft.Json
* System.Management.Automation
* Microsoft.HyperV.PowerShell

---

## Technical Highlights

### Hyper-V Infrastructure Automation

Provisioned complete virtual machine environments through PowerShell runspaces embedded directly inside C# applications.

Features include:

* VM creation
* Virtual networking
* Memory management
* CPU configuration
* Secure Boot setup
* VHDX attachment
* Firmware configuration

---

### Cross-Platform Operations

Unified Windows and Linux administration into a single interface by combining:

* PowerShell automation
* WMI queries
* Registry management
* SSH connectivity
* Log retrieval
* Remote command execution

---

### Real-Time Monitoring

Implemented asynchronous background monitoring services that continuously evaluate:

* VPN status
* Hardware configuration
* Network connectivity
* Infrastructure readiness

without blocking the application user interface.

---

## Skills Demonstrated

* Infrastructure Automation
* DevOps Tooling
* PowerShell Scripting
* Hyper-V Administration
* Linux Administration
* SSH Automation
* Configuration Management
* System Administration
* Remote Diagnostics
* Automation Engineering
* Windows Internals
* Network Troubleshooting
* Cross-Platform Operations
* Application Development
* Operational Excellence
* Process Automation

---

## Outcome

Developed a production-used internal operations platform that centralized infrastructure provisioning, configuration management, diagnostics, and troubleshooting workflows into a single automation dashboard, significantly reducing manual effort and improving operational efficiency.

