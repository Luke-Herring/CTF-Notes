### Nmap Scan 
- `nmap -p 53,135,139,88,389,445,464,593,636,3268,3269,5985,9389,49676,49696,49674,49675,49667,49666 -sV -sC -T16 -Pn -oA $IP $IP`

### Get Domain name
- `smbmap -H $IP`

### Kerberoasting
Kerberoasting is an extremely common attack in active directory environments which targets Active Directory accounts with the SPN value set.


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
- `smbmap -H $IP` list Samba shares