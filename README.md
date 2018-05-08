# guacamole-0.9.14-script-install-Centos-7
Script for installing Guacamole 0.9.14 on Centos 7 with MySql and Tomcat. Easy just follow the instructions :)

This script work in a clean CentOs 6/7 installation and install Guacamole 0.9.14 version for a local users authentication.
Task of this script.
* Install Packages dependencies
* Download Guacamole and MySQL Connector packages
* Install Guacamole Server
* Install Guacamole Client
* Install MySQL Connector
* Configure MariaDB or MySQL
* Configure FirewallD or Iptables
* Setting Tomcat Server
* Generates a Java KeyStore for SSL Support

1. Assuming you're logged in as root, type in the following to install Wget :
```bash
yum install -y wget
```
2. Let's download the script using Wget :
```sh
wget https://github.com/ROBERTPASCAL/guacamole/archive/guacamole14.tar.gz
```

3. decompress the tar file 
```sh
tar xvf guacamole14.tar.gz
cd guacamole
```
3. Now let's make sure we can execute the script :
```sh
chmod +x guacamole-install-script.sh
```
4. Execute the script :)
```sh
./guacamole-install-script.sh
```
