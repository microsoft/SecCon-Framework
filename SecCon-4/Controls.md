The controls enforced in SECCON 4 implement more controls and a more sophisticated security
configuration than SECCON 5. While they may have a slightly higher impact to
users or to applications, they enforce a level of security more commensurate
with the risks facing users with access to sensitive information. Microsoft
recommends using the Audit/Enforce methodology for controls with an Audit mode,
and the rings methodology for those that do not, with a moderate timeline that
is anticipated to be slightly longer than the process in SECCON 5.

| Feature Set                                                 | Feature                                               | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|-------------------------------------------------------------|-------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Windows Defender                                            | Enforce memory protection for OS-level controls:      | Exploit protection applies helps protect devices from malware that use exploits to spread and infect. It consists of several mitigations that can be applied at either the operating system level, or at the individual app level. There is a risk to application compatibility, as some applications may rely on blocked behavior (e.g. dynamically generating code without marking memory as executable). Microsoft recommends gradually deploying this configuration using the Rings methodology.                                            |
| Exploit Guard                                               |                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Exploit Protection                                          |                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Windows Defender                                            | Configure and Enforce Attack Surface Reduction Rules: | Attack surface reduction controls help prevent actions and apps that are typically used by exploit-seeking malware to infect machines. There is a risk to application compatibility, as some applications may rely on blocked behavior (e.g. an Office application spawning a child process). Each control has an Audit mode, and as such, Microsoft recommends the Audit / Enforce Methodology (repeated here):                                                                                                                                |
| Exploit Guard                                               |                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Attack Surface Reduction (ASR)                              |                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Windows Defender                                            | Configure and enforce Network Protection              | Network protection helps to prevent employees from using any application to access dangerous domains that may host phishing scams, exploits, and other malicious content on the Internet. It expands the scope of Windows Defender SmartScreen to block all outbound HTTP(s) traffic that attempts to connect to low-reputation sources (based on the domain or hostname). There is a risk to application compatibility, as a result of false positives in flagged sites. Microsoft recommends deploying using the Audit / Enforce Methodology. |
| Exploit Guard                                               |                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Network Protection                                          |                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

-   Control flow guard (CFG)

-   Data Execution Protection (DEP)

-   Mandatory ASLR

-   Bottom-Up ASLR

-   High-entropy ASLR

-   Validate Exception Chains (SEHOP)

-   Validate heap integrity

-   Block executable content from email client and webmail

-   Block all Office applications from creating child processes

-   Block Office applications from creating executable content

-   Block Office applications from injecting code into other processes

-   Block JavaScript or VBScript from launching downloaded executable content

-   Block execution of potentially obfuscated scripts

-   Block Win32 API calls from Office macro

-   Block executable files from running unless they meet a prevalence, age, or
    trusted list criterion

-   Use advanced protection against ransomware

-   Block credential stealing from the Windows local security authority
    subsystem (lsass.exe)

-   Block process creations originating from PSExec and WMI commands

-   Block untrusted and unsigned processes that run from USB

-   Block Office communication applications from creating child processes

-   Block Adobe Reader from creating child processes

1.  Audit – enable the controls in audit mode, and gather audit data in a
    centralized location

2.  Review – review the audit data to assess potential impact (both positive and
    negative) and configure any exemptions from the security control you need to
    configure

3.  Enforce – Deploy the configuration of any exemptions and convert the control
    to enforce mode
