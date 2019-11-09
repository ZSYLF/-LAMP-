# -LAMP-
yum install httpd

service httpd start

安装MySQL之前，先将系统上的软件更新

yum update

yum install mysql-server

service mysqld start

 /usr/bin/mysql_secure_installation
 
 命令行终端将会提示你输入 MySQL 内 root 用户的密码，然后重置 MySQL root 密码后的新密码，最后，命令行终端将会要求你更新 root 用户的密码。
 
 yum install php php-mysql
 
 vi /var/www/html/info.php
 
按i键输入下面三行代码，完成后按Esc键，然后打出：wq！退出

{<?php

phpinfo();

?>}

最后重启apache

service httpd restart 
