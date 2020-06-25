### Prerequisite

- request file from burp suite or any tool request intercept
- CREDENTIALFILE in pair of username:password format
- username field
- password field
- invalid message

### Features

 - Read request file from burp suite or any tool request intercept
 - WAF fingerprint:
	 - Mod_Security
	 - WebKnight
	 - Cloudflare
	 - FortiWeb
	 - Imperva Incapsula
	 - GoDaddy
	 - ASP.NET Generic
	  
 - Web Protection fingerprint:
	 - Clickjacking
	 - CloudFlare protection
	 - CSRF token


### Tested on 

 - http://vulnweb.lab.rz.my/user/login.php
 - https://grabme.herokuapp.com/target/


### Installation
 1. Python 3 
 1. run 'bash install.sh' to auto-install module in requirements.txt
 2. chmod +x httpwaf.py

### Usage

    usage: httpwaf.py [-h] -r REQUESTFILE -c CREDENTIALFILE -u USERFIELD -p PASSFIELD -i INVMSG [-V]
    
    Parallel Dictionary Login
    
    optional arguments:
    
          -h, --help            					show this help message and exit
          -r REQUESTFILE, --requestfile REQUESTFILE  		path to requestfile.txt format from burpsuite request intercept is compulsory!!
          -c CREDENTIALFILE, --credentialfile CREDENTIALFILE  	path to credentialfile.txt in pair of username:password format
          -u USERFIELD, --userfield USERFIELD  			username field
          -p PASSFIELD, --passfield PASSFIELD  			password field
          -i INVMSG, --invmsg INVMSG  				invalid message in double quoted string
          -V, --version         					show program's version number and exit

### Output

![enter image description here](https://raw.githubusercontent.com/faisalfs10x/HTTPwaf-Login-Bruteforce/master/1.png)
![enter image description here](https://raw.githubusercontent.com/faisalfs10x/HTTPwaf-Login-Bruteforce/master/2.png)
