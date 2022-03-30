### Nmap Scan 
- `nmap -p 53,135,139,88,389,445,464,593,636,3268,3269,5985,9389,49676,49696,49674,49675,49667,49666 -sV -sC -T16 -Pn -oA 10.10.181.245 10.10.181.245`

### Get Domain name
- `smbmap -H $IP`

### Kerberos User Enumeration
- `nmap -Pn -p 88 –script krb5-enum-users –script-args realm=’ecorp’,userdb=usernames.lst 192.168.1.22`

<!-- -->
https://wadcoms.github.io/#+No%20Creds