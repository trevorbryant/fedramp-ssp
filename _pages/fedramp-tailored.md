---
title: FEDRAMP Tailored SSP Template
permalink: /fedramp-tailored
layout: home
system-security-plan: 
  id: UUID
  metadata: 
    title: 
    published: 
    last-modified: 
    version: 
    oscal-version: 1.0
    document-ids: 
    properties: 
    links: 
    roles: 
    parties: 
    responsible-parties: 
      information-system-owner: 
        party-ids: John Doe
        properties: System Owner
        annotations: 
        links: 
        remarks:
      independent-assessor: 
        party-ids: Company X
        properties: Third Party Assessor
        annotations: 
        links: 
        remarks:
      authorizing-offical: 
        party-ids: Jane Doe
        properties: AO
        annotations: 
        links: 
        remarks:
      authorizing-offical-management-poc: 
        party-ids: Jane Doe
        properties: Management POC
        annotations: 
        links: 
        remarks:           
      authorizing-offical-technical-poc: 
        party-ids: Jane Doe
        properties: Technical POC
        annotations: 
        links: 
        remarks:
      information-system-security-officer: 
        party-ids: Jane Doe
        properties: ISSO
        annotations: 
        links: 
        remarks: 
      information-system-security-manager: 
        party-ids: Jane Doe
        properties: ISSM
        annotations: 
        links: 
        remarks:                 
    remarks: 
  import-profile: 
    href: 
    remarks: 
  system-characteristics: 
    system-ids:
    system-name: SHORTNAME-FULLSYSTEMNAME
    system-name-short: SHORTNAME
    description: "System purpose or function"
    properties: 
    annotations: 
    links: 
    date-authorized: 
    security-sensitivity-level: Low
    system-information: 
      properties: 
      annotations: 
      links: 
      information-types: 
    security-impact-level: 
      security-objective-confidentiality: fips-199-low
      security-objective-integrity: fips-199-low
      security-objective-availability: fips-199-low
    status: 
      state: operational
      remarks: "System status explained here."
    leveraged-authorizations:
      AWS:
        id: FEDRAMP-ID
        name: "Leveraged Service Provider Owner"
        properties:
        annotations:
        links:
        party-id:
        date-authorized: YYYY-MM-DD
        remarks:
      GCP:
        id: FEDRAMP-ID
        name: "Leveraged Service Provider Owner"
        properties:
        annotations:
        links:
        party-id:
        date-authorized: YYYY-MM-DD
        remarks:    
    authorization-boundary: 
      description: "Provide an explicit definition
of the system’s Authorization Boundary"
      properties: 
      annotations: 
      links: 
      diagrams:           
        AuthorizationBoundary: 
          description: 
          properties: 
          links: "https://cloud.gov/img/example-diagram-1.svg"
          caption: 
          remarks:           
      remarks: 
    network-architecture: 
      description: Optional overview of Network Architecture
      properties: 
      annotations: 
      links: 
      diagrams: 
        NetworkArchitecture: 
          description: 
          properties: 
          links: "https://cloud.gov/img/example-diagram-2.svg"
          caption: 
          remarks: 
      remarks: 
    data-flow: 
      description: Optional overview of Data Flow
      properties: 
      annotations: 
      links: 
      diagrams: 
        DataFlow: 
          description: 
          properties: 
          links: "https://cloud.gov/img/example-diagram-2.svg"
          caption: 
          remarks: 
      remarks: 
    responsible-parties: 
      ISSO: 
        party-ids: 
        properties: 
        annotations: 
        links: 
        remarks: 
    remarks: 
  system-implementation: 
    properties: 
    annotations: 
    links: 
    users: 
      sysadmin: 
        title: System Adminstrator
        short-name: 
        description: Add/remove users and hardware, install and configure software, OS updates, patches and hotfixes, perform backups.
        properties: Internal
        annotations: Privileged (P)
        links: 
        role-ids: 
        authorized-privileges: Full administrative access (root)
        remarks: Moderate
      client-adminstrator: 
        title: Client Administrator
        short-name: 
        description: Add/remote client users. Create, modify, and delete client applications.
        properties: External
        annotations: Non-Privileged (NP)
        links: 
        role-ids: 
        authorized-privileges: Portal administration
        remarks: N/A
      program-director: 
        title: Program Director
        short-name: 
        description: Reviews, approves and enforces policy.
        properties: Internal
        annotations: No Logical Access (NLA)
        links: 
        role-ids: 
        authorized-privileges: Project administration
        remarks: Limited            
    # the element below doesnt exist
    remarks: |
        "There are currently \<*number*\> internal personnel and \<*number*\> external personnel. Within one year, it is anticipated that there will be \<*number*\> internal personnel and \<*number*\> external personnel."
    components: 
      web-server: 
        name: 
        component-type: 
        description: 
        properties: 
        annotations: 
        links: 
        status: 
          state: operational
          remarks: 
        responsible-roles: 
        remarks: 
    services:
      service:
        id:
        name:
        description:
        properties:
        annotations:
        links:
        ssp-protocol:
        purpose:
        remarks:
        protocol:
            title:
            description:
            type:
            properties:
            port-ranges:
                start:
                end:
                transport:
      ssp-interconnection:
        id:
        remote-system-name:
        annotations:
        links:
        responsible-parties:
        remarks:
    system-inventory: 
      inventory-items:
        inventory-item:
          id:
          assest-id:
          description:
          properties:
          annotations:
          links:
          responsible-parties:
          remarks:
      implemented-components:
        implemented-component:
          use:
          properties:
          annotations:
          links:
          responsible-parties:
          remarks:
      remarks: 
    remarks: 
  control-implementation: 
    description: 
    implemented-requirements: 
      implemented-requirement:
        id:
        control-id:
        description:
        properties:
        annotations:
        links:
        by-components:
        responsible-roles:
        set-params:
        statements:
          statement:
            description:
            properties:
            links:
            responsible-roles:
            by-components:
            remarks:
        remarks: 
  back-matter: 
    citations: 
    resources: 
---
# FedRAMP Tailored LI-SaaS

Table of Contents
=================

* [1. Information System Name](#1-information-system-name)
* [2. Information System Categorization](#2-information-system-categorization)
   * [2.1. Information Types](#21-information-types)
   * [2.2. Security Objectives Categorization (FIPS 199)](#22-security-objectives-categorization-fips-199)
* [3. Information System Owner](#3-information-system-owner)
* [4. Independent Assessor](#4-independent-assessor)
* [5. Authorizing Official](#5-authorizing-official)
* [6. Other Designated Contacts](#6-other-designated-contacts)
* [7. Assignment of Security Responsibility](#7-assignment-of-security-responsibility)
* [8. Information System Operational Status](#8-information-system-operational-status)
* [9. Information System Type](#9-information-system-type)
   * [9.1. Cloud Service Models](#91-cloud-service-models)
   * [9.2. Cloud Deployment Models](#92-cloud-deployment-models)
   * [9.3. Leveraged Authorizations](#93-leveraged-authorizations)
* [10. General System Description](#10-general-system-description)
   * [10.1. System Function or Purpose](#101-system-function-or-purpose)
   * [10.2. Information System Components and Boundaries](#102-information-system-components-and-boundaries)
   * [10.3. Types of Users](#103-types-of-users)
   * [10.4. Network Architecture](#104-network-architecture)
* [11. System Environment](#11-system-environment)
   * [11.1. Hardware Inventory](#111-hardware-inventory)
   * [11.2. Software Inventory](#112-software-inventory)
   * [11.3. Network Inventory](#113-network-inventory)
   * [11.4. Data Flow](#114-data-flow)
   * [11.5. Ports, Protocols, and Services](#115-ports-protocols-and-services)
* [12. System Interconnections](#12-system-interconnections)
* [13. FedRAMP Applicable Laws and Regulations](#13-fedramp-applicable-laws-and-regulations)
   * [13.1. FedRAMP Tailored LI-SaaS Guidance](#131-fedramp-tailored-li-saas-guidance)
   * [13.2. APPLICABLE STANDARDS AND GUIDANCE](#132-information-system-name-applicable-standards-and-guidance)

# 1. Information System Name

This FedRAMP *Tailored* Low Impact Software as a Service (LI-SaaS)
Framework provides an overview of the security requirements for the
{{ page.system-security-plan.system-characteristics.system-name }} ({{ page.system-security-plan.system-characteristics.system-name-short }}) and
describes the controls in place or planned for implementation to provide
a level of security appropriate for the information to be transmitted,
processed, or stored by the system. Information security is vital to our
critical infrastructure and its effective performance and protection is
a key component of our national security program. Proper management of
information technology (IT) systems is essential to ensure the required
risk impact level of confidentiality, integrity, and availability of the
data transmitted, processed, or stored by the {{ page.system-security-plan.system-characteristics.system-name-short }} system is in 
place and operating as intended.

The security safeguards implemented for the {{ page.system-security-plan.system-characteristics.system-name-short }} system meet
the policy and control requirements set
forth in this FedRAMP *Tailored* LI-SaaS Framework. All systems are
subject to monitoring, consistent with applicable laws, regulations,
agency policies, procedures, and practices.

**Table 1‑1. Information System Identifier, Name, and Abbreviation**

| Unique Identifier                | Information System Name             | Information System Abbreviation       |
| -------------------------------- | ------------------------------------| ------------------------------------- |
| {{ page.system-security-plan.id }} | {{ page.system-security-plan.system-characteristics.system-name }} | {{ page.system-security-plan.system-characteristics.system-name-short }}                              |

# 2. Information System Categorization

The overall {{ page.system-security-plan.system-characteristics.system-name-short }}sensitivity categorization is recorded in Table 2.1, Security Categorization, which follows. The completed FedRAMP FIPS 199 document is included in this document as
Attachment 3 – FedRAMP FIPS Security Categorization.

**Table 2‑1. System Security Categorization**

|  **System Sensitivity Level:**                             |            |
| ----------------------------- | ---------- |
| {{ page.system-security-plan.system-characteristics.system-name }} | {{ page.system-security-plan.system-characteristics.security-sensitivity-level }} Impact |

## 2.1. Information Types

This section describes how the information types used by
{{ page.system-security-plan.system-characteristics.system-name-short }} are categorized for confidentiality, integrity, and availability of sensitivity levels.

The following tables identify the information types that are input,
stored, processed, and/or output from {{ page.system-security-plan.system-characteristics.system-name-short }}.
The selection of the information types is based on
guidance provided by the Office of Management and Budget (OMB) Federal
Enterprise Architecture (EA) Program Management Office (PMO) Business
Reference Model 2.0, National Institute of Standards and Technology
(NIST) Federal Information Processing Standard (FIPS) Publication 199,
*Standards for Security Categorization of Federal Information and
Information Systems*, and NIST Special Publication 800-60 (NIST SP
800-60) , *Guide for Mapping Types of Information and Information
Systems to Security Categories*.

FIPS 199\[1\] allows for a full range of information types. In order to
meet specific, niche needs of systems, Agencies can specify the types of
information being placed in the cloud environment. For FedRAMP
*Tailored* LI-SaaS, Agencies can specify the type(s) of information that
will reside in FedRAMP *Tailored* LI-SaaS applications/systems.

To be considered a FedRAMP *Tailored* LI-SaaS cloud application/service,
the answer to all of the following questions must be “yes:”

1.  Does the service operate in a cloud environment?

2.  Is the cloud service fully operational?

3.  Is the cloud service a Software as a Service (SaaS), as defined by
    NIST SP 800-145, The NIST Definition of Cloud Computing?

4.  Does the cloud service contain no personally identifiable
    information (PII), except as needed to provide a login capability
    (username, password and email address)?

5.  Is the cloud service low-security-impact, as defined by FIPS PUB
    199, Standards for Security Categorization of Federal Information
    and Information Systems?

6.  Is the cloud service hosted within a FedRAMP-authorized Platform as
    a Service (PaaS) or Infrastructure as a Service (IaaS), or is the
    CSP providing the underlying cloud infrastructure?

**Table 2‑3. Sensitivity Categorization of Information Types for the**
{{ page.system-security-plan.system-characteristics.system-name }}

<table>
<thead>
<tr class="header">
<th><p>Information Type</p>
<p>(Use only information types from NIST SP 800-60, Volumes I and II as amended)</p></th>
<th>NIST 800-60 identifier for Associated Information Type</th>
<th>Confidentiality</th>
<th>Integrity</th>
<th>Availability</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><em>&lt;Information Type&gt;</em></td>
<td><em>&lt;NIST Identifier&gt;</em></td>
<td><em>Low</em></td>
<td><em>Low</em></td>
<td><em>Low</em></td>
</tr>
<tr class="even">
<td><em>&lt;Information Type&gt;</em></td>
<td><em>&lt;NIST Identifier&gt;</em></td>
<td><em>Low</em></td>
<td><em>Low</em></td>
<td><em>Low</em></td>
</tr>
<tr class="odd">
<td><em>&lt;Information Type&gt;</em></td>
<td><em>&lt;NIST Identifier&gt;</em></td>
<td><em>Low</em></td>
<td><em>Low</em></td>
<td><em>Low</em></td>
</tr>
</tbody>
</table>

## 2.2. Security Objectives Categorization (FIPS 199)

Based on the information provided in Table 2.3, Sensitivity
Categorization of Information Types for the {{ page.system-security-plan.system-characteristics.system-name-short }} default to the high-water mark for the Information
Types as identified in Table 2.4, Security Impact Level, below.

If the security impact level for confidentiality, integrity, and
availability for any of the identified data types is moderate or high,
the information system is not a FedRAMP *Tailored* LI-SaaS system. The
Cloud Service Provider (CSP) must meet the standard FedRAMP Low,
Moderate, or High impact baseline security requirements, as applicable,
and complete the requirement documentation.

**Table 2‑4. Security Impact Level**

| Security Objective  | Low, Moderate or High |
| ------------------- | --------------------- |
| **Confidentiality** | {{ page.system-security-plan.system-characteristics.    security-impact-level.security-objective-confidentiality }}             |
| **Integrity**       | {{ page.system-security-plan.system-characteristics.    security-impact-level.security-objective-integrity }}                   |
| **Availability**    | {{ page.system-security-plan.system-characteristics.    security-impact-level.security-objective-availability }}                |

Through careful review and analysis, the baseline security
categorization for the {{ page.system-security-plan.system-characteristics.system-name-short }} system has
been determined and is listed in Table 2.5, Baseline Security
Configuration, which follows.

**Table 2‑5. Baseline Security Configuration**

|  **Baseline Security Configuration:**                             |            |
| ----------------------------- | ---------- |
| {{ page.system-security-plan.system-characteristics.system-name }} | {{ page.system-security-plan.system-characteristics.security-sensitivity-level }} Impact |

Using this categorization, in conjunction with the risk assessment and
any unique security requirements, the security controls for this system
have been established as detailed in this FedRAMP *Tailored* LI-SaaS
Framework.

# 3. Information System Owner 

The following individual is identified as the system owner or functional
proponent/advocate for this system.

**Table 3‑1. Information System Owner**

| Information System Owner Information |                                  |
| ------------------------------------ | -------------------------------- |
| **Name**                             | {{ page.system-security-plan.metadata.responsible-parties.information-system-owner.party-ids }}                         |
| **Title**                            | {{ page.system-security-plan.metadata.responsible-parties.information-system-owner.properties }}                        |
| **Company / Organization**           | \<Company/Organization\>.        |
| **Address**                          | \<Address, City, State and Zip\> |
| **Phone Number**                     | \<555-555-5555\>                 |
| **Email Address**                    | \<email address\>                |

# 4. Independent Assessor

The following individual is identified as the Independent Assessor for
this system.

**Table 4‑1. Independent Assessor**

| Independent Assessor Information |                                  |
| -------------------------------- | -------------------------------- |
| **Name**                         | {{ page.system-security-plan.metadata.responsible-parties.independent-assessor.party-ids }}                         |
| **Title**                        | {{ page.system-security-plan.metadata.responsible-parties.independent-assessor.properties }}                        |
| **Company / Organization**       | \<Company/Organization\>.        |
| **Address**                      | \<Address, City, State and Zip\> |
| **Phone Number**                 | \<555-555-5555\>                 |
| **Email Address**                | \<email address\>                |

# 5. Authorizing Official

The Authorizing Official (AO) or Designated Approving Authority (DAA)
for the {{ page.system-security-plan.system-characteristics.system-name-short }} system is:

| Authorizing Official             |                                  |
| -------------------------------- | -------------------------------- |
| **Name**                         | {{ page.system-security-plan.metadata.responsible-parties.authorizing-offical.party-ids }}                         |
| **Title**                        | {{ page.system-security-plan.metadata.responsible-parties.authorizing-offical.properties }}                        |
| **Company / Organization**       | \<Company/Organization\>.        |
| **Address**                      | \<Address, City, State and Zip\> |
| **Phone Number**                 | \<555-555-5555\>                 |
| **Email Address**                | \<email address\>                |

# 6. Other Designated Contacts

The individual(s) identified below possess an in-depth knowledge of this
system and/or its functions and operation.

**Table 6‑1. Information System AO Management Point of Contact**

| Information System AO Management Point of Contact |                                  |
| ------------------------------------------------- | -------------------------------- |
| **Name**                                          | {{ page.system-security-plan.metadata.responsible-parties.authorizing-offical-management-poc.party-ids }}                        |
| **Title**                                         | {{ page.system-security-plan.metadata.responsible-parties.authorizing-offical-management-poc.properties }}                        |
| **Company / Organization**                        | \<Company/Organization\>         |
| **Address**                                       | \<Address, City, State and Zip\> |
| **Phone Number**                                  | \<555-555-5555\>                 |
| **Email Address**                                 | \<email address\>                |

**Table 6‑2. Information System AO Technical Point of Contact**

| Information System AO Technical Point of Contact |                                  |
| ------------------------------------------------ | -------------------------------- |
| **Name**                                         | {{ page.system-security-plan.metadata.responsible-parties.authorizing-offical-management-poc.party-ids }}                            |
| **Title**                                        | {{ page.system-security-plan.metadata.responsible-parties.authorizing-offical-management-poc.properties }}                        |
| **Company / Organization**                       | \<Company/Organization\>         |
| **Address**                                      | \<Address, City, State and Zip\> |
| **Phone Number**                                 | \<555-555-5555\>                 |
| **Email Address**                                | \<email address\>                |


# 7. Assignment of Security Responsibility

The {{ page.system-security-plan.system-characteristics.system-name-short }} Information System Security Officer (ISSO), or their equivalent, identified below, have been appointed in writing and are deemed to have significant cyber and operational role
responsibilities.

**Table 7‑1. Internal ISSO (or Equivalent) Point of Contact**

| Internal ISSO (or Equivalent) Point of Contact |                                  |
| ---------------------------------------------- | -------------------------------- |
| **Name**                                       | {{ page.system-security-plan.metadata.responsible-parties.information-system-security-manager.party-ids }}                        |
| **Title**                                      | {{ page.system-security-plan.metadata.responsible-parties.information-system-security-manager.properties }}                             |
| **Company / Organization**                     | \<Company/Organization\>         |
| **Address**                                    | \<Address, City, State and Zip\> |
| **Phone Number**                               | \<555-555-5555\>                 |
| **Email Address**                              | \<email address\>                |

**Table 7‑2. AO ISSO Point of Contact**

| AO ISSO Point of Contact |                                  |
| ------------------------ | -------------------------------- |
| **Name**                 | {{ page.system-security-plan.metadata.responsible-parties.information-system-security-officer.party-ids }}                         |
| **Title**                | {{ page.system-security-plan.metadata.responsible-parties.information-system-security-officer.properties }}                             |
| **Organization**         | \<Company/Organization\>.        |
| **Address**              | \<Address, City, State and Zip\> |
| **Phone Number**         | \<555-555-5555\>                 |
| **Email Address**        | \<email address\>                |

# 8. Information System Operational Status

The system is currently in the life-cycle phase shown in Table 8.1, System Status, which follows. Only operational systems can be granted an Authority to Operate (ATO).

**Table 8‑1. System Status**

| System Status |                      |
| ------------- | -------------------- |
| Operational     | The system is operating and in production.                   |
| Under Development  | The system is being designed, developed, or implemented. |
| Major Modification | The system is undergoing a major change, development, or transition. |
| Other              | Explaination required                                   |

{{ page.system-security-plan.system-characteristics.system-name }} is {{ page.system-security-plan.system-characteristics.status.state | capitalize }}

>{{ page.system-security-plan.system-characteristics.status.remarks }}


# 9. Information System Type

The {{ page.system-security-plan.system-characteristics.system-name-short }} system makes use of unique managed service provider architecture layer(s).

## 9.1. Cloud Service Models

Information systems, particularly those based on cloud architecture models, are made up of different service layers. Below are some questions that can help system owners determine if their system is a cloud followed by specific questions to help system owners determine the
type of cloud.

**Table 9‑1. Determining a Cloud System**

| Question (Yes/No)                                                                               | Conclusion                                                                                                                                                             |
| ----------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Does the system use virtual machines (VM)?                                                      | A no response means that system is most likely not a cloud.                                                                                                            |
| Does the system have the ability to expand its capacity to meet customer demand?                | A no response means that the system is most likely not a cloud.                                                                                                        |
| Does the system allow the customer to build anything other than servers?                        | A no response means that the system is an Infrastructure as a Service (IaaS). A yes response means that the system is either a Platform as a Service (PaaS) or a SaaS. |
| Does the system offer the ability to create databases?                                          | A yes response means that the system is a PaaS.                                                                                                                        |
| Does the system offer various developer toolkits and Application Programming Interfaces (APIs)? | A yes response means that the system is a PaaS.                                                                                                                        |
| Does the system offer only applications that are available by obtaining a login?                | A yes response means that system is a SaaS. A no response means that the system is either a PaaS or an IaaS.                                                           |

The layers of the {{ page.system-security-plan.system-characteristics.system-name-short }} defined in this FedRAMP *Tailored* LI-SaaS Framework are indicated in Table 9.2, Service
Layers Represented in this FedRAMP *Tailored* LI-SaaS Framework, which
follows.

**Table 9‑2. Service Layers Represented in this FedRAMP Tailored LI-SaaS Framework**

| Service Provider Architecture Layers |                              |                   |
| ------------------------------------ | ---------------------------- | ----------------- |
| - [ X ]                                 | Software as a Service (SaaS) | Major Application |

## 9.2. Cloud Deployment Models

Information systems are made up of different deployment models. The
deployment models of the {{ page.system-security-plan.system-characteristics.system-name-short }} that are
defined in this FedRAMP Tailored LI-SaaS Framework, and that are not leveraged by any other FedRAMP Authorizations, are indicated in Table
9.3, Cloud Deployment Model Represented in this FedRAMP *Tailored* LI-SaaS Framework, which follows.

**Table 9‑3. Cloud Deployment Model Represented in this FedRAMP Tailored LI-SaaS Framework**

<table>
<thead>
<tr class="header">
<th><strong>Service Provider Cloud Deployment Model</strong></th>
<th></th>
<th></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td></td>
<td>Public</td>
<td>Cloud services and infrastructure supporting multiple organizations and agency clients.</td>
</tr>
<tr class="even">
<td></td>
<td>Private</td>
<td>Cloud services and infrastructure dedicated to a specific organization/agency and no other clients.</td>
</tr>
<tr class="odd">
<td></td>
<td>Government Only Community</td>
<td>Cloud services and infrastructure shared by several organizations/agencies with same policy and compliance considerations.</td>
</tr>
<tr class="even">
<td></td>
<td>Hybrid</td>
<td><p>Explain: (e.g., cloud services and infrastructure that provides private cloud for secured applications and data where required and public cloud for other applications and data).</p>
<p>Explain</p></td>
</tr>
</tbody>
</table>

## 9.3. Leveraged Authorizations

The {{ page.system-security-plan.system-characteristics.system-name-short }} leverages a pre-existing
FedRAMP Authorized IaaS and/or PaaS. FedRAMP Authorizations leveraged by
this {{ page.system-security-plan.system-characteristics.system-name-short }} are listed in Table 9.4,
Leveraged Authorizations, which follows.

Table 9‑4. Leveraged Authorizations

| Leveraged Information System Name         | Leveraged Service Provider Owner | Date Granted |
| ----------------------------------------- | -------------------------------- | ------------ |
| *\<Leveraged information system name 1\>* | *\<Service provider owner 1\>*   | *\<Date\>*   |
| *\<Leveraged information system name 2\>* | *\<Service provider owner 2\>*   | *\<Date\>*   |
| *\<Leveraged information system name 3\>* | *\<Service provider owner 3\>*   | *\<Date\>*   |

{{ page.system-security-plan.system-characteristics.system-name-short }} leverages
{{ page.system-security-plan.system-characteristics.leveraged-authorizations | newline_to_br }}

# 10. General System Description

This section includes a general description of the {{ page.system-security-plan.system-characteristics.system-name }}.

## 10.1. System Function or Purpose

{{ page.system-security-plan.system-characteristics.description }}

## 10.2. Information System Components and Boundaries

{{ page.system-security-plan.system-characteristics.authorization-boundary.description }}

A detailed and explicit definition of the system authorization boundary diagram is represented in Figure 10.1, Authorization Boundary Diagram,
below.

[**Figure 10‑1. Authorization Boundary Diagram**]({{ page.system-security-plan.system-characteristics.authorization-boundary.diagrams.AuthorizationBoundary.links }})

![Authorization Boundary Diagram]({{ page.system-security-plan.system-characteristics.authorization-boundary.diagrams.AuthorizationBoundary.links }})

## 10.3. Types of Users

All personnel have their status categorized with a sensitivity level in accordance with PS-2. Personnel (employees or contractors) of service providers are considered Internal Users. All other users are considered External Users. User privileges (authorization permission after authentication takes place) are described in Table 10.1, Personnel Roles and Privileges, which follows.

**Table 10‑1. Personnel Roles and Privileges**

| Role                      | Internal or External | Privileged (P), Non-Privileged (NP), or No Logical Access (NLA) | Sensitivity Level | Authorized Privileges             | Functions Performed                                                                                               |
{% for user in page.system-security-plan.system-implementation.users %}
| {{ user }} | {{ user.properties }} | {{ user.annotations }} | {{ user.remarks }} | {{ user.authorized-privileges }} | {{ user.description }} |
{% endfor %}

{{ page.system-security-plan.system-implementation.users.remarks }}

## 10.4. Network Architecture

Assessors should be able to easily map hardware, software, and network inventories back to this diagram. The logical network topology is shown in Figure 10.2, Network Diagram, mapping the data flow between components. 

Figure 10.2, Network Diagram(s), provides a visual depiction of the system network components that constitute the {{ page.system-security-plan.system-characteristics.system-name-short }} system.

{{ page.system-security-plan.system-characteristics.network-architecture.description }}

[**Figure 10‑2. Network Diagram**]({{ page.system-security-plan.system-characteristics.network-architecture.diagrams.NetworkArchitecture.links }})

![Network Diagram]({{ page.system-security-plan.system-characteristics.network-architecture.diagrams.NetworkArchitecture.links }})

# 11. System Environment 

The FedRAMP Inventory Workbook is included in this document in
ATTACHMENT 2 – FedRAMP Inventory Workbook.

## 11.1. Hardware Inventory

Use the FedRAMP Inventory Workbook to list the principal hardware components for {{ page.system-security-plan.system-characteristics.system-name }}.

Note: A complete and detailed list of the system hardware and software inventory is required per NIST SP 800-53, Rev 4 CM-8.

## 11.2. Software Inventory

Use the FedRAMP Inventory Workbook to list the principal software components for {{ page.system-security-plan.system-characteristics.system-name }}.

## 11.3. Network Inventory 

Use the FedRAMP Inventory Workbook to list the principal network devices and components for {{ page.system-security-plan.system-characteristics.system-name }}.

## 11.4. Data Flow 

The data flow in and out of the system boundaries is represented in Figure 11.1, Data Flow Diagram, below.

{{ page.system-security-plan.system-characteristics.data-flow.description }}

[**Figure 11‑1. Data Flow Diagram**]({{ page.system-security-plan.system-characteristics.data-flow.diagrams.DataFlow.links }})

![Data Flow Diagram]({{ page.system-security-plan.system-characteristics.data-flow.diagrams.DataFlow.links }})

## 11.5. Ports, Protocols, and Services 

Table 11.1, Ports, Protocols, and Services, lists the ports, protocols, and services enabled for the {{ page.system-security-plan.system-characteristics.system-name-short }}.

**Table 11‑1. Ports, Protocols, and Services**

| Ports (TCP/UDP)  | Protocols       | Services       | Purpose       | Used By       |
| ---------------- | --------------- | -------------- | ------------- | ------------- |
{% for service in page.system-security-plan.system-implementation. %}
| {{ user }} | {{ user.properties }} | {{ user.annotations }} | {{ user.remarks }} | {{ user.authorized-privileges }} | {{ user.description }} |
{% endfor %}

# 12. System Interconnections

Table 12.1, System Interconnections, is consistent with the CA-3 Authorized Connections attestation information.

TODO - make forloop

**Table 12‑1. System Interconnections**

<table>
<thead>
<tr class="header">
<th>SP IP Address and Interface</th>
<th>External Organization Name and IP Address of System</th>
<th>External Point of Contact and Phone Number</th>
<th>Connection Security (IPSec VPN, SSL, Certificates, Secure File Transfer etc.)</th>
<th><p>Data Direction</p>
<p>(incoming, outgoing, or both)</p></th>
<th>Information Being Transmitted</th>
<th>Port or Circuit Numbers</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><em>&lt;SP IP Address / Interface&gt;</em></td>
<td><em>&lt;External Org/IP&gt;</em></td>
<td><p><em>&lt;External Org POC&gt;</em></p>
<p><em>&lt;Phone 555-555-5555&gt;</em></p></td>
<td><em>&lt;Connection Security&gt;</em></td>
<td><em>Choose an item.</em></td>
<td><em>&lt;Information Transmitted&gt;</em></td>
<td><em>&lt;Port/Circuit Numbers&gt;</em></td>
</tr>
<tr class="even">
<td><em>&lt;SP IP Address / Interface&gt;</em></td>
<td><em>&lt;External Org/IP&gt;</em></td>
<td><p><em>&lt;External Org POC&gt;</em></p>
<p><em>&lt;Phone 555-555-5555&gt;</em></p></td>
<td><em>&lt;Connection Security&gt;</em></td>
<td><em>Choose an item.</em></td>
<td><em>&lt;Information Transmitted&gt;</em></td>
<td><em>&lt;Port/Circuit Numbers&gt;</em></td>
</tr>
<tr class="odd">
<td><em>&lt;SP IP Address / Interface&gt;</em></td>
<td><em>&lt;External Org/IP&gt;</em></td>
<td><p><em>&lt;External Org POC&gt;</em></p>
<p><em>&lt;Phone 555-555-5555&gt;</em></p></td>
<td><em>&lt;Connection Security&gt;</em></td>
<td><em>Choose an item.</em></td>
<td><em>&lt;Information Transmitted&gt;</em></td>
<td><em>&lt;Port/Circuit Numbers&gt;</em></td>
</tr>
<tr class="even">
<td><em>&lt;SP IP Address / Interface&gt;</em></td>
<td><em>&lt;External Org/IP&gt;</em></td>
<td><p><em>&lt;External Org POC&gt;</em></p>
<p><em>&lt;Phone 555-555-5555&gt;</em></p></td>
<td><em>&lt;Connection Security&gt;</em></td>
<td><em>Choose an item.</em></td>
<td><em>&lt;Information Transmitted&gt;</em></td>
<td><em>&lt;Port/Circuit Numbers&gt;</em></td>
</tr>
<tr class="odd">
<td><em>&lt;SP IP Address / Interface&gt;</em></td>
<td><em>&lt;External Org/IP&gt;</em></td>
<td><p><em>&lt;External Org POC&gt;</em></p>
<p><em>&lt;Phone 555-555-5555&gt;</em></p></td>
<td><em>&lt;Connection Security&gt;</em></td>
<td><em>Choose an item.</em></td>
<td><em>&lt;Information Transmitted&gt;</em></td>
<td><em>&lt;Port/Circuit Numbers&gt;</em></td>
</tr>
<tr class="even">
<td><em>&lt;SP IP Address / Interface&gt;</em></td>
<td><em>&lt;External Org/IP&gt;</em></td>
<td><p><em>&lt;External Org POC&gt;</em></p>
<p><em>&lt;Phone 555-555-5555&gt;</em></p></td>
<td><em>&lt;Connection Security&gt;</em></td>
<td><em>Choose an item.</em></td>
<td><em>&lt;Information Transmitted&gt;</em></td>
<td><em>&lt;Port/Circuit Numbers&gt;</em></td>
</tr>
</tbody>
</table>

# 13. FedRAMP Applicable Laws and Regulations

The FedRAMP Laws and Regulations Template can be found on this page:
<https://www.fedramp.gov/templates/>.

## 13.1. FedRAMP Tailored LI-SaaS Guidance

Table 13.1, FedRAMP *Tailored* LI-SaaS Applicable Guidance, includes additional documentation specific to FedRAMP *Tailored* LI-SaaS information systems.

Table 13‑1. FedRAMP Tailored LI-SaaS Applicable Guidance

| Title                                                                                                                     | Date      |
| ------------------------------------------------------------------------------------------------------------------------- | --------- |
| FedRAMP *Tailored* Security Requirements for Low Impact Software as a Service (LI-SaaS) Cloud Systems                     | 1/30/2017 |
| NIST SP 800-171 rev 1, Protecting Controlled Unclassified Information in Nonfederal Information Systems and Organizations | 12/2016   |
| NIST Framework for Improving Critical Infrastructure Cybersecurity, v1.0                                                  | 2/12/2014 |

.

## 13.2. APPLICABLE STANDARDS AND GUIDANCE 

Table 13.2, {{ page.system-security-plan.system-characteristics.system-name-short }} Standards and Guidance,
includes any additional standards and guidance specific to
{{ page.system-security-plan.system-characteristics.system-name-short }}.

**Table 13‑2. {{ page.system-security-plan.system-characteristics.system-name-short }} Standards and Guidance**

| Identification Number | Title               | Date         | Link               |
| --------------------- | ------------------- | ------------ | ------------------ |
| \<Reference ID\>      | \<Reference Title\> | \<Ref Date\> | \<Reference Link\> |
| \<Reference ID\>      | \<Reference Title\> | \<Ref Date\> | \<Reference Link\> |
| \<Reference ID\>      | \<Reference Title\> | \<Ref Date\> | \<Reference Link\> |

1.  FIPS Pub 199: FEDERAL INFORMATION PROCESSING STANDARDS PUBLICATION:
    Standards for Security Categorization of Federal Information and
    Information Systems, February 2004;
    [<span class="underline">http://csrc.nist.gov/publications/fips/fips199/FIPS-PUB-199-final.pdf</span>](http://csrc.nist.gov/publications/fips/fips199/FIPS-PUB-199-final.pdf)
| Identification Number | Title               | Date         | Link               |
| --------------------- | ------------------- | ------------ | ------------------ |
| \<Reference ID\>      | \<Reference Title\> | \<Ref Date\> | \<Reference Link\> |
| \<Reference ID\>      | \<Reference Title\> | \<Ref Date\> | \<Reference Link\> |
| \<Reference ID\>      | \<Reference Title\> | \<Ref Date\> | \<Reference Link\> |

1.  FIPS Pub 199: FEDERAL INFORMATION PROCESSING STANDARDS PUBLICATION:
    Standards for Security Categorization of Federal Information and
    Information Systems, February 2004;
    [<span class="underline">http://csrc.nist.gov/publications/fips/fips199/FIPS-PUB-199-final.pdf</span>](http://csrc.nist.gov/publications/fips/fips199/FIPS-PUB-199-final.pdf)