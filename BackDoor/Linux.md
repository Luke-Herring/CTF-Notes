				SSH BackDoor

-- ssh-keygen                                   Generates ssh key
    -- Leave public key                      	 Place '/root/.ssh'
    -- SSH Name                                    Name 'authorized_keys'
        -- chmod 600 id_rsa               	  Gives permissions

-- ssh -i id_rsa root@ip                    Use BackDoor

				PHP BackDoor

-- Location                                         /var/www/html
    -- BackDoor script                           Script/PHP-BackDoor.php

-- Where to execute script                https://ip/PHP-BackDoor.php

                		Hide script

-- Add in existing PHP File
-- Change the "cmd" parameter, cmd is very obvious

				Cronjob BackDoor
-- crontab -l
-- Add to Cronjob                               /script/Crontab Line 1
    -- Add Script inside Cronjob            /script/Crontab Line 3,4
-- Get Bash shell

-- Host HTTP server                             python3 -m http.server 8080

				Links

-- https://airman604.medium.com/9-ways-to-backdoor-a-linux-box-f5f83bae5a3c
