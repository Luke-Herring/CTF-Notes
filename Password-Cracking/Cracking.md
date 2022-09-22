				Linux Hashing /etc/shadow
-- $1$   MD5
-- $2a$ Blowfish
-- $2y$ Eksblowfish
-- $5$   SHA-256
-- $6$   SHA-512      

				cewl
- Make a wordlist by crawling the website



cewl -w list.txt -d 5 -m 5 www.Ip.com 			

				Haiti
Identify what type of hash
`haite $HASH`

				ssh2john
- Convert private key to hash
`python3 ssh2john.py privatekey > privatekey.hash`
- Use john to crack hash
`john privatekey.hash -w=/wordlist`

<!-- -->

				Default passwords
www.cirt.net/passwords
www.default-password.info
www.datarecovery.com/rd/default-passwords/