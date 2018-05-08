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
wget https://github.com/ROBERTPASCAL/guacamole/archive/release-9.14.tar.gz
```
3. decompress the tar file 
```sh
tar xvf release-9.14.tar.gz
cd guacamole-release-9.14
```
4. Now let's make sure we can execute the script :
```sh
chmod +x guacamole-install-script.sh
```
5. Execute the script :)
```sh
./guacamole-install-script.sh
```
6. check with getenforce the level of selinux. It's must be permissive :
```sh
getenforce
```
you can change it with this command :
```sh
setenforce 0
sed -i -e 's/^SELINUX=.*/SELINUX=disable/' /etc/sysconfig/selinux
```
*A big hug to the creator of that script : correo@nacimientohernan.com.ar*
