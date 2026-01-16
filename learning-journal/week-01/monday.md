# Week 1, Day 1 - Microsoft Entra ID Fundamentals

## Key Concepts Learned

### 1. Entra ID vs. Windows Server AD
**Main Difference**: [Main Difference:
Microsoft Entra ID is a Microsoft-managed, cloud-based identity and access management service, while Active Directory Domain Services (AD DS) is an on-premises directory service that runs on Windows Server domain controllers.

Entra ID is used to manage identities for Azure, Microsoft 365, and SaaS applications, and it supports modern authentication methods such as Multi-Factor Authentication (MFA), Conditional Access, passwordless sign-in, and protocols like SAML, OAuth 2.0, OpenID Connect, and WS-Federation. Entra ID is internet-facing and communicates primarily over HTTPS (port 443).

AD DS, on the other hand, is designed for on-premises environments, managing domain-joined computers, file shares, printers, and legacy applications within a local network.]
**AQUAPINE Impact**: [For AQUAPINE Consult, Entra ID provides a centralized and scalable identity management system for its approximately 45 employees across Lagos and Ibadan. It enables role-based access control (RBAC), Conditional Access, and Multi-Factor Authentication to ensure employees only access resources required for their job roles.

Entra ID also supports Single Sign-On (SSO) across company applications, improves security visibility through sign-in logs and audit trails, and helps AQUAPINE meet compliance and data protection requirements while reducing IT administrative overhead]

### 2. Tenant Hierarchy
**What is a tenant?**: [A tenant is a dedicated Microsoft Entra ID instance that acts as an organization’s identity boundary. It stores all Entra ID objects such as users, groups, devices, and application registrations.
]
**AQUAPINE Tenant Name**: aquapineconsult.onmicrosoft.com
**Why this structure matters**: [The tenant defines the security, identity, and access boundary for AQUAPINE. All authentication, authorization, and policy enforcement occur within this tenant, making it critical for access control, auditing, and governance.]

### 3. User Types
**Cloud-Only Users**: [Users created directly in Entra ID with no on-premises dependency. Example: IT administrators or office staff created directly in the cloud.]
**Synchronized Users**: [Users that originate from an on-premises Active Directory and are synchronized to Entra ID using Azure AD Connect. This would apply if AQUAPINE later deploys on-premises infrastructure.]
**Guest Users**: [External users invited into the tenant for collaboration, such as vendors or consultants, with limited access permissions.]

### 4. Groups
**Security Groups**: [Used to assign permissions to Azure resources and applications efficiently.]
**Microsoft 365 Groups**: [Used for collaboration services such as Outlook, Microsoft Teams, and SharePoint]
**AQUAPINE Group Strategy**: [Ibadan-Farm-Operations, Ibadan-Microbiology-Lab, Lagos-HR-Department, Lagos-IT-Admin. This structure supports role-based access control and operational separation between departments and locations.]

## Business Context Questions

1. Why can't AQUAPINE just use personal email accounts?
   [Personal email accounts introduce significant security risks, including lack of centralized access control, no enforced MFA or Conditional Access, no auditing capability, and difficulty revoking access when employees leave the company.]

2. How does Entra ID help with the Ibadan-Lagos separation?
   [Entra ID enables logical separation using groups, administrative units, and role-based access, allowing each location to be managed independently while remaining under one centralized identity system.]

3. What happens if a microbiologist leaves the company?
   [If Entra ID is implemented, the IT administrator can immediately disable or delete the user account and remove the user from all groups, instantly revoking access to all company systems. This enforces proper identity lifecycle management.

Without Entra ID, access removal would be inconsistent, delayed, or incomplete, creating a security risk.]

## Questions for Instructor
- [ ] [Question 1]: I would like a deeper explanation of Microsoft Entra Domain Services, including when and why an organization should use it.

- [ ] [Question 2]: I want to clearly understand Shared Mailboxes, Microsoft Teams channels, and SharePoint sites, including their purpose and how AQUAPINE would use them operationally.

