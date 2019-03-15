The behaviors recommended in SECCON 4 implement a more sophisticated security
process. While they may require a more sophisticated organization, they enforce
a level of security more commensurate with the risks facing users with access to
sensitive information.

| Feature Set| Feature  | Description  |
|---------------------|----------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Antivirus  | Configure Protection Updates to failover to retrieval from Microsoft | Sources for Windows Defender Antivirus Protection Updates can be provided in an ordered list. If you are using internal distribution, such as SCCM or WSUS, configure Microsoft Update lower in the list as a failover.  |
| OS Security Updates | Deploy Windows Quality Updates within 4 days | As the time between release of a patch and an exploit based on the reverse engineering of that patch continues to shrink, engineering a process that provides the ability to validate and deploy quality updates addressing known security vulnerabilities is a critical aspect of security hygiene.|
| Helpdesk| 1:1 Administration| A simple and common model for helpdesk support is to add the Helpdesk group as a permanent member of the Local Administrators group of every device. If any device is compromised and helpdesk can connect to it, then these credentials can be used to obtain privilege on any / all other devices. Design and implement a strategy to provide helpdesk support without providing 1:all admin access – constraining the value of these Helpdesk credentials |
