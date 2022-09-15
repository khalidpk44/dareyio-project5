# dareyio-project5 
1. Create and configure two Linux-based virtual servers (EC2 instances in AWS) Server A name - `mysql server`
Server B name - `mysql client`
2. On mysql server Linux Server install MySQL Server software 
3. sudo apt update
4. sudo apt install mysql-server
5. sudo systemctl start mysql.service
6. login to the mysql server (sudo mysql)
7. change the password for the root user (ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';)
8. exit mysql server (exit)
9. open the mysql configuration file on mysql server (sudo vi /etc/mysql/mysql.conf.d/mysqld.cnf)
10 replace the bind-address from 127.0.0.1 to 0.0.0.0
11. restart mysql service (service mysql restart)
12. login to mysql server (mysql)
13. create a new user into mysql server (CREATE USER 'user'@'%' IDENTIFIED BY 'password';)
14. grant full access to new user (GRANT ALL PRIVILEGES ON *.* TO 'user'@'%' WITH GRANT OPTION;)
15. Flush privileges (FLUSH PRIVILEGES;)
16. On mysql client Linux Server install MySQL Client software
17. sudo apt update
18. sudo apt install mysql-client
19. logon into mysql server using mysql client (mysql -u user -p  -h <mysql server private or public ip>)
20. supply password for mysql user and press enter

  
  
