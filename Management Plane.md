# Management Plane

Provides the tools (web interface and APIs) necessary to configure, monitor, and control your cloud environment. 

Provides virtual management options equivalent to the physical administration options a legacy data center would provide. (e.g. Powering VMs on/off, provisioning VM resources, migrating a VM)

You interact with the management plane through tools, including the CSPs cloud portal, Powershell, or other command line, or other client SDKs

Seperate from and works with the **control plane** and the **data plane**. 

> **Control Plane** is what you are calling when you create top-level cloud resources with ARM & Bicep (Azure), CloudFormation (AWS) or Terraform. (Infrastructure as code)

> **Data Plane** performs operations on resources create dthrough the control plane. 

# Securing the Management Plane

## Key interfaces for the management plane

**Cloud Portal**. The main website interface for the CSP platform. (Azure Portal, AWS Management Console, Google Cloud Console)

**Scheduling**. The ability to stop/start a resource at a scheduled time. (Instance scheduler or Lambda AWS, Azure Automation or Functions)

**Orchestration**. Automating processes to manage resources, services, and workloads, and Infrastructure-as-Code (IaC) deployments. (Cloud Formation(AWS), Azure DevOps, Cloud Build(GCP))

**Maintenance**. update, upgrad, security patching, etc. 

> Secure the management plane interfaces with multi-factor auth (MFA) role-based access control (RBAC), and role management. 