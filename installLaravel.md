##Install Laravel in linux with ubuntu or similar distro

### 1. Install Apache Web Server
To check, we have to run the following command.
```
sudo systemctl status apache2
```
If no run Apache service installed, install it:
```
sudo apt install apache2
```
Verify in web:

check this site:

http://localhost/

#### Important commands:
```
## Start command ##
    sudo systemctl start apache2.service
## Stop command ##
   sudo systemctl stop apache2.service
## Restart command ##
   sudo systemctl restart apache2.service
```
### 2. Install PHP
Execute the command below:
```
sudo apt install php libapache2-mod-php php-mbstring php-xmlrpc php-soap php-gd php-xml php-cli php-zip php-bcmath php-tokenizer php-json php-pear
```
Update your packages:
```
sudo apt-get update
sudo apt-get upgrade
```
Install PHP:
```
sudo apt-get install php
```
After instalation check version:
```
php --version
```
## Fix errors with instalation laravel

### requires ext-curl
For those who use php8.1
```
sudo apt-get install php8.0-curl
```
Or simply run below command to install by your version:
```
sudo apt-get install php-curl
```
