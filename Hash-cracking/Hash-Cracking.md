				John the Ripper
-- john --wordlist=[filename] [passwordfile] --format=
-- john --show [filename]

				Hydra
/Scripts
				
				Linux Hashing /etc/shadow
-- md5crypt $1$, MD5(Unix)
-- bcrypt $2*$, Blowfish(Unix)
-- sha256crypt $5$, SHA256(Unix)
-- sha512crypt $6$, SHA512(Unix)

				Windows Hashing
--LM
--NTLM

   				Misc Tools

-- python ssh2john.py id_rsa > id_rsa.john					SSH2john
-- unshadow passwd-file.txt shadow-file.txt > unshadowed.txt 	Unshadow
-- fcrackzip -vbDp rockyou.txt -u ./backup.zip				      Zip cracking

 				Links				
-- https://crackstation.net/									
-- http://openwall.info/wiki/john/sample-hashes
