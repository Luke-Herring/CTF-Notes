### Allows Gobuster to enumerate website directories.
`gobuster dir --wordlist=/usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt --url $IP t 100`

### Allows Gobuster to brute-force subdomains.
`gobuster dns -d site.com -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt`

-Other subdomain
`host -t axfr site.com $IP`

### Allows Gobuster to brute-force virtual hosts
`gobuster vhost -u $IP -w /usr/share/wordlists/seclists/Discovery/DNS/subdomains-top1million-5000.txt`