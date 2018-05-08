# guacamole 0.9.14 script install CentOs7
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
```
yum install -y wget
```
2. Let's download the script using Wget :
```
wget -q https://github.com/ROBERTPASCAL/guacamole/releases/download/release-9.14/guacamole-install-script.sh
```
4. Now let's make sure we can execute the script :
```
chmod +x guacamole-install-script.sh
```
5. Execute the script :)
```
./guacamole-install-script.sh
```
**A big hug to the creator of that script : correo@nacimientohernan.com.ar**
