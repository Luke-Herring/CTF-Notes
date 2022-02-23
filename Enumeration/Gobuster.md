					Dir
### Allows the user to enumerate website directories.
`gobuster dir --wordlist=/usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt --url $IP t 100`

					DNS
### Allows Gobuster to brute-force subdomains.
`gobuster dns -d site.com -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt`

					Vhosts
### Allows Gobuster to brute-force virtual hosts
`gobuster vhost -u $IP -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt`