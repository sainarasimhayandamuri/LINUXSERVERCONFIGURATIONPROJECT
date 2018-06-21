# Udacity-Linux-Server-Configuration
### About
  This is the Udacity project 5 about the Configuring the Linux the server.In this project, a Linux virtual machine needs to be configurated to support the Item Catalog website.

### Server Details
Server IP Address 13.232.21.104

Hosted site Url [http://13.232.21.104.xip.io/](http://13.232.21.104.xip.io/)

### Procedure
1. Launch your Virtual Machine with your Udacity account
2. Follow the instructions provided to SSH into your server
3. Create a new user named grader
4. Give the grader the permission to sudo
5. Update all currently installed packages
6. Change the SSH port from 22 to 2200
7. Configure the Uncomplicated Firewall (UFW) to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)
8. Configure the local timezone to UTC
9. Install and configure Apache to serve a Python mod_wsgi application
10. Install and configure PostgreSQL:
	- Do not allow remote connections
	- Create a new user named catalog that has limited permissions to your catalog application database
11. Install git, clone and setup your Catalog App project (from your GitHub repository from earlier in the Nanodegree program) so that it functions correctly when visiting your server’s IP address in a browser. Remember to set this up appropriately so that your .git directory is not publicly accessible via a browser!


### How to connect as grader:
  save private key provided in your local machine and run the following command
  ```
  ssh -i path/to/privatekey -p 2200 grader@13.232.21.104
    
  ```
### ID_rsa key
 
 ```
 -----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAw7LSEyrnhboT6YQ011q4XBBuywzmvqpQlaoPFID3pOpL+Q22
Cyu7D9XX5iHbECXIuJP/jYHHp4HDVD+5YqjiUWcYz2mUdBbwoFHR1qDpCh/z1Ldm
b4qYmgnzp7NEC/mJYxQ6aany1ihz+HaVbZM9Wk2/yHJgGKZUX7Yjbutax/jjG8xv
44m9Z4Iqir9g0CorXT4hqnzJcx9byeLUT3qRptzMziAPMfcQjQWNhbnzghwDB3W/
slbBLbAWmG9Wj89J4C4nikljbLm1dGfDFW3G3pSYEWEMzTWQDGTe+H0qLMkOtJUy
4eV4b7yhP69i+F/cX5FcLRwxNvlZfq/58Tqp9QIDAQABAoIBAD0VS8z/z1RGSIDS
60ts3a6e0nY+iKdqscyFUD+uIZ4wI5aRWQkTlUfUD5edaasYoBY8279nitIWBsn9
Ofg5jqqp62ySH+w8XM8turmrcBHg91KmDCs0r30lLhBiPBMgyGlMnw7sJQgDiG89
VFbnZncRXZNLYANRp3RYfabZf3R7B1pY5ep/+sByRCmOfLlib6yBVspKdEbVYC8k
qlxgPTyqfJYCjfRY1ylKuF4irjtLC/YoFE6b94z16y1eKBVZIi6RI512Qcq/lsfC
7X8zENdzkHbbGmXg1hwCxz/2DzfhqRwJDxJktvlLeyOdw9ssrWRMAyXszfeycErd
4VtdTQECgYEA51p+L0iM9WL9eewrFBQCG0mvYw6Z4hWUwvW1zts/+Xg/qX+2IfxM
F9SnOb+fb2cKRe0nNuAjBDW+48FaI1fIOzxOrs+3t0qVjqtAC2yrqspFi7ezcZTp
77BbFer0eMkQ5opp6uCJ5o5m3hFqMSTUOkTZam8I/3briRNFbxQhujkCgYEA2Ivw
o63V+F52A96FZ14oJlDRFMO3q8eLgqV1400M67f6bnz6pYoU87AJAaq7wBnztnre
koyEWwrLwMPxlxeTBu9R4N5JmOX0E3ijsm0ub6VS2o/MBrvPIXNBHAQOdb7QrFky
c2m7kLQmwH0mw/xi+n7rHHfksPFoHr68lfYLHZ0CgYB85UmB1TTjtFEK5QhMipCo
kprwaw2AFA5/QY6o4Ywj7VrQ8nUs27tokhDFCEHWLlZJccHdyhqdRzaKVfOHaPhb
oi8ICHMxrD4ZCzJD+KKkTRZGWyGwi6fPEfHaX0Ejg8hv7QFJH3bS1MWL1PLzHOLF
oi2NW+wLnfOByLmPQdsDYQKBgC3UQBOEANrVswhSmc0sojapt/Y7Da4vRxlZRz/Z
2Lgyca/ch3dtZ83DHcTai222kFu4WU6OqpxSBpk/XuvpM1auY5fBs7XGRQex6oMi
lEdQp95VvIpYSRf9OnRhb2YAAk3XetPuNqIDXogydHfZ/GCjZ8LYpO/Fx5FqMKNU
NToJAoGAVVukCVgUjjQ1oa4fwMBzU8qFVkFlmM7YHgqaLPtHX3U9/dxARqNuktg2
BJThNgqPrSuS+XTvFuCbt2NKImDs3IYZ1UgCnrF9jq/HgDgn/ytc+R63rg1AwzIW
3cmiSEG7AhqR1L61EtuVpngQRfnGGasEaUXKjVv7zLaAAbamznQ=
-----END RSA PRIVATE KEY-----
 ```
 
### Id_rsa.pub key
```
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDDstITKueFuhPphDTXWrhcEG7LDOa+qlCVqg8UgPek6kv5DbYLK7sP1dfmIdsQJci4k/+NgcengcNUP7liqOJRZxjPaZR0FvCgUdHWoOkKH/PUt2ZvipiaCfOns0QL+YljFDppqfLWKHP4dpVtkz1aTb/IcmAYplRftiNu61rH+OMbzG/jib1ngiqKv2DQKitdPiGqfMlzH1vJ4tRPepGm3MzOIA8x9xCNBY2FufOCHAMHdb+yVsEtsBaYb1aPz0ngLieKSWNsubV0Z8MVbcbelJgRYQzNNZAMZN74fSosyQ60lTLh5XhvvKE/r2L4X9xfkVwtHDE2+Vl+r/nxOqn1 sai narasimha@DESKTOP-F8RMTCQ

```
### Configuring Linux Server

#### Updating all packages
```
sudo apt-get update
sudo apt-get upgrade
```

#### Creating grader User:
  ```
  sudo adduser grader 
  ```

###  grader password
  ```
  vinay
  ```

  ```
  This will add you to new user
  ```
  sudo nano /etc/sudoers
  ```
  Below the Root user append the following line
  ```
  grader  ALL=(ALL:ALL) ALL
  ```
  This will grant sudo permission to grader
  #### Creating a ssh key pair for grader
   On your local machine in terminal/command prompt
   ```
   ssh-keygen
   ```
   This will generate public and private ssh keys which is saved to .ssh folder
   
   Then in your virtual machine change to newly created user
   ```
   su - grader
   ```
   Create a new directory .ssh and new file authorized_keys in that directory
   ```
   mkdir .ssh
   sudo nano .ssh/authorized_keys
   ```
   Copy the public key with .pub extension to authorized_keys and save the file
   ```
   chmod 700 .ssh
   chmod 644 .ssh/authorized_keys
   ```
   - 700 will give read write and execute permission to user.
   - 644 prevent other user from writting in to file.
   Then restart ssh server
   ```
   service ssh restart
   ```
   
   Now from your log in to grader with private key generated 
   ```
   ssh -i .ssh/id_rsa grader@ipaddress 
   ```
  #### Changing the ssh port to 2200
   ```
   sudo nano /etc/ssh/sshd_config
   ```
   Change port 22 to port 2200
    
   Restart the ssh server
   
   ```
   service ssh restart
   ```
   
   >Note: Before Logging using ssh add custom TCP port 2200 under lightsaail firewall in networking tab in lightsail instance console  
   
   Now Login using command like this
   ```
   ssh -i .ssh/id_rsa -p 2200 grader@ipaddress
   ```
   
  #### Disabling ssh login as root
  `sudo nano /etc/ssh/sshd_config`
  
  make change `PermitRootLogin no`
  
  #### Configurating  Ufw firewall
  ```
  sudo ufw allow 2200/tcp
  sudo ufw allow 80/tcp
  sudo ufw allow 123/udp
  sudo ufw enable
  ```
  This will allow all required ports and enables the ufw
  
  After that 
  ```
  sudo ufw status
  ```
  It will display all allowed ports
  
  #### Changing time Zone
  `sudo dpkg-reconfigure tzdata`
  
  select none from list and then select utc.
  
  #### Installing Apache2 
  In terminal 
  
  ```sudo apt-get install apache2```
  
  Now mod_wsgi
  
  ```sudo apt-get install python-setuptools libapache2-mod-wsgi```
  
  Enable mod_wsgi
  
  ```sudo a2enmod wsgi ```
  ##### Setting up your flask application to work with apache2
   Creating a flask app
   
   In /var/www directory create a new folder
   `sudo mkdir FlaskApp`
   
   Install git 
   
   `sudo apt-get install git`
   
   move to the FlaskApp `cd FlaskApp`
   
   In that direcory clone your github repository
   
   `sudo git clone https://github.com/username/catalog.git`
   
   Rename your repository to FlaskApp
   
   Then rename your project file to `__init__.py`
   
   >Error : While accesssing the client_secrets.json file 
   ```
   PROJECT_ROOT = os.path.realpath(os.path.dirname(__file__))
   json_url = os.path.join(PROJECT_ROOT, 'client_secrets.json')
   CLIENT_ID = json.load(open(json_url))['web']['client_id']
   ```
   Use json_url instead client_secrets.json in script
   
   Reffered from [stack overflow](https://stackoverflow.com/questions/44742566/wsgi-cant-find-file-in-same-directory-in-app)
   
  ##### Install and configuring postgresql for project
   Install Postgres `sudo apt-get install postgresql`
   
   login to postgres `sudo su - postgres`
   
   postgres shell `psql`
   
   create user `CREATE USER catalog WITH PASSWORD 'password';`
   
   permit user to createdb `ALTER USER catalog CREATEDB;`
   
   Create a db name  catalog with user catalog `CREATE DATABASE catalog WITH OWNER catalog;`
   
   connect to db `\c catalog`
   
   revoke all permission to public `REVOKE ALL ON SCHEMA public FROM public;`
   
   Give schema permission to user catalog `GRANT ALL ON SCHEMA public TO catalog;`
   
   exit from db and postgres `\q and exit`
   
   Change the database connection in both db_setup.py and `__init__.py` as `engine =       create_engine('postgresql://catalog:password@localhost/catalog')`
   
   Now you are ready with your applicatiom
  #### Configure and Enable a New Virtual Host
   `sudo nano /etc/apache2/sites-available/FlaskApp.conf`
   
   In this add the following code
   ```
   <VirtualHost *:80>
		ServerName mywebsite.com
		ServerAdmin admin@mywebsite.com
		WSGIScriptAlias / /var/www/FlaskApp/flaskapp.wsgi
		<Directory /var/www/FlaskApp/FlaskApp/>
			Order allow,deny
			Allow from all
		</Directory>
		Alias /static /var/www/FlaskApp/FlaskApp/static
		<Directory /var/www/FlaskApp/FlaskApp/static/>
			Order allow,deny
			Allow from all
		</Directory>
		ErrorLog ${APACHE_LOG_DIR}/error.log
		LogLevel warn
		CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>
   ```
   Enable the virtual host 
   `sudo a2ensite FlaskApp`
   
   Disabling the default apache2 page
   `sudo a2dissite 000-default.conf`
   
  #### Create the .wsgi File
    ```
    cd /var/www/FlaskApp
    sudo nano flaskapp.wsgi 
    ```
   Add the following code
   
   ```
   #!/usr/bin/python
    import sys
    import logging
    logging.basicConfig(stream=sys.stderr)
    sys.path.insert(0,"/var/www/FlaskApp/")

    from FlaskApp import app as application
    application.secret_key = 'Add your secret key'
   ```
   save and exit
   
   Deploying flask app with apache2 is referred from [Digital ocean](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)
   
   #### Installing require modules
   You can either install all modules on your machine or create a virtual environment for the project and install the modules
   ` pip install flask sqlalchemy psycopg2 requests oauth2client`
   
   #### Setting up your Google Oauth2
   Login to your [developer console](https://console.developers.google.com) and select your project and edit OAuth details as following
   
   Javascript origin
   `http://ip.xip.io`
   
   redirect URI
   
   `http://ip.xip.io\login`
   
   `http://ip.xip.io\gconnect`
   
   `http://ip.xip.io\callback`
   
   [xip.io](xip.io) is a free DNS which will be the same as using IP address
   
   #### Final Step
   Restart your apache2 server
   
   `sudo service apache2 restart`
   
