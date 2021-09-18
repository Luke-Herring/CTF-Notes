				Find World Writable Folders
-- find / -x dev -type d -perm -0002 -ls 2> /dev/null


				Find SUID
-- find / -user root -perm /4000

				Sudo
-- Sudo -l

				Cronjobs
-- cat /etc/crontab								

				/etc/passwd
-- cat /etc/passwd

-- openssl passwd newpasswordhere		Changes root password

				Misc
-- cat ~/.*history | less						
-- ls -la /									

				Links
-- https://gtfobins.github.io/
