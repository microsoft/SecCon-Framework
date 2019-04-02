The controls enforced in SECCON 3 implement complex security configuration and controls. 
They are likely to have a higher impact to users or to applications,
enforcing a level of security commensurate with the risks facing the most targeted organizations. 
Microsoft recommends using the Audit/Enforce methodology for controls with audit mode, and the rings methodology for those that do
not.

| Feature Set  | Feature  | Description  |
|--------------|----------|--------------|
| Exploit protection  | Enable exploit protection | Exploit protection helps protect devices from malware that use exploits to spread and infect to other devices. It consists of several mitigations that can be applied at the individual app level.  |
| Windows Defender Application Control (WDAC) *or* AppLocker | Configure devices to use application whitelisting using one of the following approaches:<br>- AaronLocker (admin writeable areas) when software distribution is not always centralized<br>*or*<br>- Managed installer when all software is pushed through software distribution<br>*or*<br>- Explicit control when the software on a device is static and tightly controlled  | Application control is a crucial line of defense for protecting enterprises given today’s threat landscape, and it has an inherent advantage over traditional antivirus solutions. Specifically, application control moves away from the traditional application trust model where all applications are assumed trustworthy by default to one where applications must earn trust in order to run. Application Control can help mitigate these types of security threats by restricting the applications that users can run and the code that runs in the System Core (kernel). WDAC policies also block unsigned scripts and MSIs, and Windows PowerShell runs in Constrained Language Mode. |



