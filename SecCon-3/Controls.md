The controls enforced in SECCON 3 implement complex security configuration and
controls. They are likely to have a higher impact to users or to applications,
enforcing a level of security commensurate with the risks facing the most
targeted organizations. Microsoft recommends using the Audit/Enforce methodology
for controls with an Audit mode, and the Rings methodology for those that do
not.

| Feature Set  | Feature  | Description  |
|--------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Windows Defender  | Enforce the Common Apps Exploit Protection provided in the Exploit Guard Evaluation Package, available at <https://aka.ms/mp7z2w> | Exploit protection applies helps protect devices from malware that use exploits to spread and infect. It consists of several mitigations that can be applied at the individual app level.  |
| Exploit Guard  |  |  |
| Exploit Protection  |  |  |
| Windows Defender  | Configure devices to use application whitelisting using one of the following approaches:  | Application control is a crucial line of defense for protecting enterprises given today’s threat landscape, and it has an inherent advantage over traditional antivirus solutions. Specifically, application control moves away from the traditional application trust model where all applications are assumed trustworthy by default to one where applications must earn trust in order to run. Application Control can help mitigate these types of security threats by restricting the applications that users can run and the code that runs in the System Core (kernel). WDAC policies also block unsigned scripts and MSIs, and Windows PowerShell runs in Constrained Language Mode. |
| Application Control  |  |  |
| *or*  |  |  |
| AppLocker  |  |  |

- AaronLocker (admin writeable areas) when not all software is available /
  distributed to through software distribution  
  *or*

- Managed Installer when all software is pushed through software distribution  
  *or*

- Explicit Control when the software on a device is static and tightly
  controlled
