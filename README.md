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
MIIEpQIBAAKCAQEAzWcNvdP/h8+fU8eaQO4zvSjrD6Fb0wQ2w29Fqua1VMh6h16G
XP0Ggs+xZ4P23NgFPlIbhAbYCr7dmrfMxAkds1BQw9ZK5eSnU7SNikKbHglrTPnQ
3xyZ6RLumrClSbMTLK9eNPyjlblGgSjJfYugIZyZk9dr7NQpe4brYPyOzMZ6La0F
Dg/yt+xzx3rWTbX2C3Dgu8p42hibTjVYaxF8nljbCKagY5deaSKGEWjBVXFre+t6
xeWzMGy7RnPtnEd6IT3egAUnQpjwmh2NfhEYeMO6r8tHZktlLi0ZaOGGO2c2fKxY
T2Ixv8TKj12KPxxCCAb0/mk7uvoYTiPkRi5NmQIDAQABAoIBADtMTQNIeLTUk8K0
FSw5mGY7seDJTKEWzliNfydfg2n+lqEOAOxHf+Gz5BtmVZZcJude/OKYtzYi9Ab+
mPbfStvBjA99hhHoeQYJUfNgVzfMsFWAqXQ/5Y8MECZIaO9l61szJZdWeEN5QYl4
JPNBo/EQLKYpwtaUSYWH5dwSDYfAH/6iVk8eFT8D6ks/8icYgHBFCuRosZxmoUik
AzQ7poPJooEgAty+sSh5CUYShbfiEHNLTtu5ZK7XQp+ZUcotX6pQUkHBHE0Rgqjh
H8DyNm+OsiainLiAihnKZ2M6nthszVg+MQC2eewqfoOkc1GlMUGBycVqR89d4Jhl
EJWEfIECgYEA+3P9JMzWx+dmnckM5qmcCaavnb/j0/wPVtDIdVoNYy3OtDld2NNW
ZkHHaLogK477sWXgh1xw9itp8VAKioH+c++9lXqlnFDr8vAHwjjXMrqSOoJhSXs4
ikFKjjr8N+EOGcutFQhBykouYjQLRvhblRXPu/54nVhCeKPuWo1/Cu0CgYEA0R3j
+7q5KY4LZJBsBdghnXjsMTZOC4Xr2y1cRf/SDYpMzLZalgfztetAB5iBCaxgLnxI
nxob3Q6XY8tijINnF2iZHqtEgfv9GJXKxYFiSAFz1Pgzf8U5kl6W+PjUESc0/QP5
Lyi3epU+XjT2YGuMkgK8bZ4jv3yCzO9NH0gKe90CgYEA4W6MXeizCgdALWdpBIa8
2L4ypce6Nnu9OMT3YpY4eFlB/ruLkm9t/0EryI1NeB+5MMK4OEK9F0W2tlxfBuwi
NsiRfCi3vtuhnWxqWErjS5yOqpvnIpyxBOoiMD9bjbFcFe5PHxMHAJfe27XzAk54
tMEYO1+ZvN66wTOe5loCssUCgYEAh17bLCUXIoByfZpEY5AjSqZx9/WYljsOkKcP
mbzehKdnygmuIHtrV/O/Umt19QYiiVUpSd2D9hkxBYgu9plFzlCG9uSWB7NRh23I
gwyby9Ms4cv+wpKxD0CuaOPjnGsOEVBWKiIojHE6m4+bgpV8vTSKOEfsClSW9AVh
noNrTf0CgYEAu6dQ9blHDU5P7U03THiLTApNWToKY4SVEcJXeFBPtpwAvTm+Y9lf
fPktaScM0+dTVo5Bc47V189VMsPzJzH+hgPcZ4vg872uVvAYf5fT+cfEBxCtJQN6
TT+XMyY6IBOXdR88uFK7mQo2NUduOgTASn4nghSZsME6KIPF0GVox1w=
-----END RSA PRIVATE KEY-----

 ```
 
### Id_rsa.pub key
```
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDNZw290/+Hz59Tx5pA7jO9KOsPoVvTBDbDb0Wq5rVUyHqHXoZc/QaCz7Fng/bc2AU+UhuEBtgKvt2at8zECR2zUFDD1krl5KdTtI2KQpseCWtM+dDfHJnpEu6asKVJsxMsr140/KOVuUaBKMl9i6AhnJmT12vs1Cl7hutg/I7MxnotrQUOD/K37HPHetZNtfYLcOC7ynjaGJtONVhrEXyeWNsIpqBjl15pIoYRaMFVcWt763rF5bMwbLtGc+2cR3ohPd6ABSdCmPCaHY1+ERh4w7qvy0dmS2UuLRlo4YY7ZzZ8rFhPYjG/xMqPXYo/HEIIBvT+aTu6+hhOI+RGLk2Z sai narasimha@DESKTOP-F8RMTCQ

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

### passphrase password

  ```
  there is no passphrase password for my project(you can directly press enter) or else press grader password.
 
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
   
