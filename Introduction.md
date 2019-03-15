Introducing the SECCON Framework
================================

Security configuration is complex. With thousands of group policies available in
Windows, choosing the “best” setting is difficult. It’s not always obvious which
permutations of policies are required to implement a complete scenario, and
there are often unintended consequences of some security lockdowns.

Because of this, with each release of Windows, Microsoft publishes [Windows
Security
Baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines),
an industry-standard configuration that is broadly known and well-tested.
However, many organizations have discovered that this baseline sets a very high
bar. While appropriate for organizations with very high security needs such as
those persistently targeted by Advanced Persistent Threats, some organizations
have found that the cost of navigating the potential compatibility impact of
this configuration is prohibitively expensive given their risk appetite. They
can’t justify the investment in that very high level of security with an ROI. As
such, Microsoft is introducing a new taxonomy for Security Configurations for
Windows 10: The SECCON Baselines.

The SECCON Baselines organizes devices into one of 5 distinct security
configurations:

| SECCON 5  | SECCON 4  | SECCON 3  | | SECCON 2  | SECCON 1  |
|----------------------|-------------------------|----------------------------------|---|-----------------------------------|--------------------------------------|
| Enterprise Security  | Enterprise  | Enterprise Cutting-Edge Security | | Server and Service Administration | Identity and Security Administration |
|  | High Security  |  | |  |  |
| Productivity Devices |  | Privileged Access Workstations | |  |  |

The SECCON Baselines divide configuration into Productivity Devices and
Privileged Access Workstations. This document will focus on Productivity Devices
(SECCON 5, 4, and 3). Microsoft’s current guidance on Privileged Access
Workstations can be found at <http://aka.ms/cyberpaw> and as part of the
Securing Privileged Access roadmap found at <http://aka.ms/privsec>.

Microsoft recommends reviewing and categorizing your devices, and then
configuring them using the prescriptive guidance for that SECCON level. SECCON 5
should be considered the minimum baseline for an enterprise device, and
increasing the protection based on both threat environment and risk appetite.

Security Control Classification
-------------------------------

This document groups recommendations into 3 categories:

| Policies  | Controls  | Behaviors  |
|------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| Microsoft recommends enforcing the configuration of the specified policies in the manner described, to harden Windows to the designated level of security. | Microsoft recommends enabling the security controls specified in the manner described, to provide protections appropriate to the designated level of security. | Microsoft recommends changing organizational behavior towards the endpoint in the manner described. |

Security Control Deployment Methodologies
-----------------------------------------

The way Microsoft recommends implementing these controls depends on the
auditability of the control– there are two primary methodologies:

| Rings  | Audit / Enforce  |
|---------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------|
| Security controls which don’t support an audit mode should be deployed gradually. A typical deployment methodology: | Security controls which support an audit mode can be deployed using the following methodology: |

1.  Test ring – deploy to a lab to validate “must test” apps prior to any
  enforcement of configuration

2.  Pilot ring – deploy to a representative sample of 2 – 5% of the environment

3.  Fast ring – deploy to the next 25% of the organization

4.  Slow ring – deploy to the remainder of the organization

5.  Audit – enable the control in audit mode, and gather audit data in a
  centralized location

6.  Review – review the audit data to assess potential impact (both positive and
  negative) and configure any exemptions from the security control you need to
  configure

7.  Enforce – Deploy the configuration of any exemptions and convert the control
  to enforce mode
