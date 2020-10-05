# MySQL ![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)

## Installation of MySQL
### Debian
```
sudo apt-get install mysql-server
```
### CentOS
```
yum localinstall https://dev.mysql.com/get/mysql57-community-release-el7-9.noarch.rpm

yum install mysql-community-server
```

## Start MySQL server
### Debian 
```
sudo service mysql start
```
### CentOS
```
sudo service mysqld start
```


## Enter into mysql from command line
### As root
```
sudo mysql -uroot -p
```
### Add a new user (after entering as root)


## Check status of MySQL server
### Debian
```
sudo systemctl status  mysql
```
### CentOS
```
sudo systemctl status mysqld
```

## Stop MySQL server
```
sudo systemctl stop  mysql
```

## Uninstall
```
sudo apt-get remove --purge mysql*
```

