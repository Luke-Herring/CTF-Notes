				Osint on people
- Instagram
- Facebook
- Twitter
- Reddit
- LinkdIn(LinkdIn forces you use your real name)

<!-- -->

				Osint on company's

https://www.crunchbase.com/				
https://sam.gov/content/home
https://www.gsaelibrary.gsa.gov/ElibMain/home.do

				WebOSINT

[Whois Registration](https://www.whois.com)
[archive.org](https://archive.org/)

				Geolocating images
-- Always use `Yandex` for reverse image search

- Language
- what side are cars on?
- license plates
- clothes

<!-- -->

				Subdomain

### SSL/TLS Certificates
[crt.sh](https://crt.sh/)

### Search engines
`site:*.website.com` will reveals subdomains

### DNS Bruteforce
using dnsrecon `dnsrecon -t brt -d website.com`

### sublist3r
`python3 /opt/sublist3r.py -d DOMAIN`

### Virtual Hosts

```
ffuf -w /usr/share/wordlists/SecLists/Discovery/DNS/namelist.txt -H "Host:FUZZ.website.com" -u http://$IP
```