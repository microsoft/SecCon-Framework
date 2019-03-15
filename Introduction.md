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

![SECON Framework](images\seccon-framework.png)

The SECCON Baselines divide configuration into Productivity Devices and
Privileged Access Workstations. This document will focus on Productivity Devices
(SECCON 5, 4, and 3). Microsoft’s current guidance on [Privileged Access
Workstations](http://aka.ms/privsec) are part of the
[Securing Privileged Access roadmap](http://aka.ms/privsec).

Microsoft recommends reviewing and categorizing your devices, and then
configuring them using the prescriptive guidance for that SECCON level. SECCON 5
should be considered the minimum baseline for an enterprise device, and Microsoft recommends
increasing the protection based on both threat environment and risk appetite.

Security Control Classification
-------------------------------

This document groups recommendations into 3 categories:

![Security Control Classifications](images\security-control-classification.png)


Security Control Deployment Methodologies
-----------------------------------------

The way Microsoft recommends implementing these controls depends on the
auditability of the control– there are two primary methodologies:

![Security Control Deployment methodologies](images\security-control-deployment-methodologies.png) 


