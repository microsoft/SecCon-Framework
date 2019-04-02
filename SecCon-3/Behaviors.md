The behaviors recommended in SECCON 3 represent the most sophisticated security
configuration. Removing admin rights can be difficult, but it is essential to
achieve a level of security commensurate with the risks facing the most targeted
organizations.

| Feature Set  | Feature  | Description  |
|--------------|----------|--------------|
| Remove Admin Rights | Remove as many users as possible from the local Administrators group, targeting 0. Microsoft recommends removing admin rights role by role. Some roles are more challenging, including:<br>- Developers, who often install rapidly iterating software which is difficult to package using current software distribution systems<br>- Scientists/ Doctors, who often must install and operate specialized hardware devices<br>- Remote locations with slow web links, where administration is delegated<br>It is typically easier to address these roles later in the process.<br>Microsoft recommends identifying the dependencies on admin rights and systematically addressing them:<br>- Legitimate use of admin rights: crowdsourced admin, where a new process is needed to complete that workflow<br>- Illegitimate use of admin rights: app compat dependency, where app remediation is the best path. The [Desktop App Assure](https://techcommunity.microsoft.com/t5/Windows-IT-Pro-Blog/What-is-Desktop-App-Assure/ba-p/270232) program can assist with these app issues | Running as non-admin limits your exposure. When you are an admin, every program you run has unlimited access to your computer. If malicious code finds its way to one of those programs, it also gains unlimited access. When an exploit runs with admin privileges, its ability to compromise your system is much greater, its ability to do so without detection is much greater, and its ability to attack others on your network is greater than it would be with only User privileges. If you’re running as admin, an exploit can:<br>- Install kernel-mode rootkits and/or keyloggers<br>- Install and start services<br>- Install ActiveX controls, including IE and shell add-ins<br>- Access data belonging to other users<br>- Cause code to run whenever anybody else logs on (including capturing passwords entered into the Ctrl-Alt-Del logon dialog)<br>- Replace OS and other program files with trojan horses<br>- Disable/uninstall antivirus<br>- Cover its tracks in the event log<br>- Render your machine unbootable |









