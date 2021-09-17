				Find World Writable Folders
-- find / -x dev -type d -perm -0002 -ls 2> /dev/null


				Find SUID
-- find / -perm -4000 -user root -exec ls -ld {} \; 2> /dev/null sudo -l
-- find / -user root -perm /4000

				Sudo
-- Sudo -l

				Cronjobs
-- cat /etc/crontab								

				/etc/passwd
-- cat /etc/passwd								any hashes to crack?

-- openssl passwd newpasswordhere				Changes root password

				Misc
-- cat ~/.*history | less						Past Commands
-- ls -la /										Hidden directory



-- https://gtfobins.github.io/
