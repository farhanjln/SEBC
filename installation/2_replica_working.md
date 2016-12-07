Connected, host fingerprint: ssh-rsa 2048 E4:9E:6D:B6:17:24:5C:28:B7:2E:CE:06:75:D4:7F:46
Last login: Wed Dec  7 04:22:13 2016 from 173.194.93.96
[hinotamashi94@instance-3 ~]$ java -version
-bash: java: command not found
[hinotamashi94@instance-3 ~]$ sudo yum install mariadb mariadb-server
Loaded plugins: fastestmirror
Loading mirror speeds from cached hostfile
 * base: chicago.gaminghost.co
 * extras: mirrors.gigenet.com
 * updates: mirror.steadfast.net
Resolving Dependencies
--> Running transaction check
---> Package mariadb.x86_64 1:5.5.50-1.el7_2 will be installed
---> Package mariadb-server.x86_64 1:5.5.50-1.el7_2 will be installed
--> Processing Dependency: perl-DBI for package: 1:mariadb-server-5.5.50-1.el7_2.x86_64
--> Processing Dependency: perl-DBD-MySQL for package: 1:mariadb-server-5.5.50-1.el7_2.x86_64
--> Processing Dependency: perl(Data::Dumper) for package: 1:mariadb-server-5.5.50-1.el7_2.x86_64
--> Processing Dependency: perl(DBI) for package: 1:mariadb-server-5.5.50-1.el7_2.x86_64
--> Processing Dependency: libaio.so.1(LIBAIO_0.4)(64bit) for package: 1:mariadb-server-5.5.50-1.el7_2.x86_64
--> Processing Dependency: libaio.so.1(LIBAIO_0.1)(64bit) for package: 1:mariadb-server-5.5.50-1.el7_2.x86_64
--> Processing Dependency: libaio.so.1()(64bit) for package: 1:mariadb-server-5.5.50-1.el7_2.x86_64
--> Running transaction check
---> Package libaio.x86_64 0:0.3.109-13.el7 will be installed
---> Package perl-DBD-MySQL.x86_64 0:4.023-5.el7 will be installed
---> Package perl-DBI.x86_64 0:1.627-4.el7 will be installed
--> Processing Dependency: perl(RPC::PlServer) >= 0.2001 for package: perl-DBI-1.627-4.el7.x86_64
--> Processing Dependency: perl(RPC::PlClient) >= 0.2000 for package: perl-DBI-1.627-4.el7.x86_64
---> Package perl-Data-Dumper.x86_64 0:2.145-3.el7 will be installed
--> Running transaction check
---> Package perl-PlRPC.noarch 0:0.2020-14.el7 will be installed
--> Processing Dependency: perl(Net::Daemon) >= 0.13 for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Net::Daemon::Test) for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Net::Daemon::Log) for package: perl-PlRPC-0.2020-14.el7.noarch
--> Processing Dependency: perl(Compress::Zlib) for package: perl-PlRPC-0.2020-14.el7.noarch
--> Running transaction check
---> Package perl-IO-Compress.noarch 0:2.061-2.el7 will be installed
--> Processing Dependency: perl(Compress::Raw::Zlib) >= 2.061 for package: perl-IO-Compress-2.061-2.el7.noarch
--> Processing Dependency: perl(Compress::Raw::Bzip2) >= 2.061 for package: perl-IO-Compress-2.061-2.el7.noarch
---> Package perl-Net-Daemon.noarch 0:0.48-5.el7 will be installed
--> Running transaction check
---> Package perl-Compress-Raw-Bzip2.x86_64 0:2.061-3.el7 will be installed
---> Package perl-Compress-Raw-Zlib.x86_64 1:2.061-4.el7 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

================================================================================================================
 Package                             Arch               Version                       Repository           Size
================================================================================================================
Installing:
 mariadb                             x86_64             1:5.5.50-1.el7_2              updates             8.9 M
 mariadb-server                      x86_64             1:5.5.50-1.el7_2              updates              11 M
Installing for dependencies:
 libaio                              x86_64             0.3.109-13.el7                base                 24 k
 perl-Compress-Raw-Bzip2             x86_64             2.061-3.el7                   base                 32 k
 perl-Compress-Raw-Zlib              x86_64             1:2.061-4.el7                 base                 57 k
 perl-DBD-MySQL                      x86_64             4.023-5.el7                   base                140 k
 perl-DBI                            x86_64             1.627-4.el7                   base                802 k
 perl-Data-Dumper                    x86_64             2.145-3.el7                   base                 47 k
 perl-IO-Compress                    noarch             2.061-2.el7                   base                260 k
 perl-Net-Daemon                     noarch             0.48-5.el7                    base                 51 k
 perl-PlRPC                          noarch             0.2020-14.el7                 base                 36 k

Transaction Summary
================================================================================================================
Install  2 Packages (+9 Dependent packages)

Total download size: 21 M
Installed size: 108 M
Is this ok [y/d/N]: y
Downloading packages:
(1/11): libaio-0.3.109-13.el7.x86_64.rpm                                                 |  24 kB  00:00:00     
(2/11): perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64.rpm                                   |  32 kB  00:00:00     
(3/11): perl-Compress-Raw-Zlib-2.061-4.el7.x86_64.rpm                                    |  57 kB  00:00:00     
(4/11): perl-DBD-MySQL-4.023-5.el7.x86_64.rpm                                            | 140 kB  00:00:00     
(5/11): perl-Data-Dumper-2.145-3.el7.x86_64.rpm                                          |  47 kB  00:00:00     
(6/11): perl-DBI-1.627-4.el7.x86_64.rpm                                                  | 802 kB  00:00:00     
(7/11): perl-Net-Daemon-0.48-5.el7.noarch.rpm                                            |  51 kB  00:00:00     
(8/11): mariadb-server-5.5.50-1.el7_2.x86_64.rpm                                         |  11 MB  00:00:00     
(9/11): mariadb-5.5.50-1.el7_2.x86_64.rpm                                                | 8.9 MB  00:00:00     
(10/11): perl-IO-Compress-2.061-2.el7.noarch.rpm                                         | 260 kB  00:00:00     
(11/11): perl-PlRPC-0.2020-14.el7.noarch.rpm                                             |  36 kB  00:00:00     
----------------------------------------------------------------------------------------------------------------
Total                                                                            28 MB/s |  21 MB  00:00:00     
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : perl-Data-Dumper-2.145-3.el7.x86_64
 Installing : libaio-0.3.109-13.el7.x86_64                                                                2/11 
  Installing : perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64                                                  3/11 
  Installing : 1:perl-Compress-Raw-Zlib-2.061-4.el7.x86_64                                                 4/11 
  Installing : perl-IO-Compress-2.061-2.el7.noarch                                                         5/11 
  Installing : perl-Net-Daemon-0.48-5.el7.noarch                                                           6/11 
  Installing : perl-PlRPC-0.2020-14.el7.noarch                                                             7/11 
  Installing : perl-DBI-1.627-4.el7.x86_64                                                                 8/11 
  Installing : perl-DBD-MySQL-4.023-5.el7.x86_64                                                           9/11 
  Installing : 1:mariadb-5.5.50-1.el7_2.x86_64                                                            10/11 
  Installing : 1:mariadb-server-5.5.50-1.el7_2.x86_64                                                     11/11 
  Verifying  : 1:mariadb-5.5.50-1.el7_2.x86_64                                                             1/11 
  Verifying  : perl-Net-Daemon-0.48-5.el7.noarch                                                           2/11 
  Verifying  : 1:mariadb-server-5.5.50-1.el7_2.x86_64                                                      3/11 
  Verifying  : perl-Data-Dumper-2.145-3.el7.x86_64                                                         4/11 
  Verifying  : perl-PlRPC-0.2020-14.el7.noarch                                                             5/11 
  Verifying  : 1:perl-Compress-Raw-Zlib-2.061-4.el7.x86_64                                                 6/11 
  Verifying  : perl-Compress-Raw-Bzip2-2.061-3.el7.x86_64                                                  7/11 
  Verifying  : perl-DBI-1.627-4.el7.x86_64                                                                 8/11 
  Verifying  : libaio-0.3.109-13.el7.x86_64                                                                9/11 
  Verifying  : perl-DBD-MySQL-4.023-5.el7.x86_64                                                          10/11 
  Verifying  : perl-IO-Compress-2.061-2.el7.noarch                                                        11/11 
Installed:
  mariadb.x86_64 1:5.5.50-1.el7_2                     mariadb-server.x86_64 1:5.5.50-1.el7_2                    
Dependency Installed:
  libaio.x86_64 0:0.3.109-13.el7                         perl-Compress-Raw-Bzip2.x86_64 0:2.061-3.el7           
  perl-Compress-Raw-Zlib.x86_64 1:2.061-4.el7            perl-DBD-MySQL.x86_64 0:4.023-5.el7                    
  perl-DBI.x86_64 0:1.627-4.el7                          perl-Data-Dumper.x86_64 0:2.145-3.el7                  
  perl-IO-Compress.noarch 0:2.061-2.el7                  perl-Net-Daemon.noarch 0:0.48-5.el7                    
  perl-PlRPC.noarch 0:0.2020-14.el7                     
Complete!
[hinotamashi94@instance-3 ~]$ sudo service mariadb status
Redirecting to /bin/systemctl status  mariadb.service
● mariadb.service - MariaDB database server
   Loaded: loaded (/usr/lib/systemd/system/mariadb.service; disabled; vendor preset: disabled)
   Active: inactive (dead)
[hinotamashi94@instance-3 ~]$ sudo service mariadb start
Redirecting to /bin/systemctl start  mariadb.service
[hinotamashi94@instance-3 ~]$ sudo service mariadb status
Redirecting to /bin/systemctl status  mariadb.service
● mariadb.service - MariaDB database server
   Loaded: loaded (/usr/lib/systemd/system/mariadb.service; disabled; vendor preset: disabled)
   Active: active (running) since Wed 2016-12-07 07:20:29 UTC; 5s ago
  Process: 2780 ExecStartPost=/usr/libexec/mariadb-wait-ready $MAINPID (code=exited, status=0/SUCCESS)
  Process: 2699 ExecStartPre=/usr/libexec/mariadb-prepare-db-dir %n (code=exited, status=0/SUCCESS)
 Main PID: 2779 (mysqld_safe)
   CGroup: /system.slice/mariadb.service
           ├─2779 /bin/sh /usr/bin/mysqld_safe --basedir=/usr
           └─3212 /usr/libexec/mysqld --basedir=/usr --datadir=/var/lib/mysql --plugin-dir=/usr/lib64/mysql/p...
Dec 07 07:20:18 instance-3 mariadb-prepare-db-dir[2699]: The latest information about MariaDB is available...g/.
Dec 07 07:20:18 instance-3 mariadb-prepare-db-dir[2699]: You can find additional information about the MyS...at:
Dec 07 07:20:18 instance-3 mariadb-prepare-db-dir[2699]: http://dev.mysql.com
Dec 07 07:20:18 instance-3 mariadb-prepare-db-dir[2699]: Support MariaDB development by buying support/new...aDB
Dec 07 07:20:18 instance-3 mariadb-prepare-db-dir[2699]: Corporation Ab. You can contact us about this at ...om.
Dec 07 07:20:18 instance-3 mariadb-prepare-db-dir[2699]: Alternatively consider joining our community base...rt:
Dec 07 07:20:18 instance-3 mariadb-prepare-db-dir[2699]: http://mariadb.com/kb/en/contributing-to-the-mari...ct/
Dec 07 07:20:18 instance-3 mysqld_safe[2779]: 161207 07:20:18 mysqld_safe Logging to '/var/log/mariadb/ma...og'.
Dec 07 07:20:18 instance-3 mysqld_safe[2779]: 161207 07:20:18 mysqld_safe Starting mysqld daemon with dat...ysql
Dec 07 07:20:29 instance-3 systemd[1]: Started MariaDB database server.
Hint: Some lines were ellipsized, use -l to show in full.
[hinotamashi94@instance-3 ~]$ sudo /usr/bin/mysql_secure_installation
/usr/bin/mysql_secure_installation: line 379: find_mysql_client: command not found

NOTE: RUNNING ALL PARTS OF THIS SCRIPT IS RECOMMENDED FOR ALL MariaDB
      SERVERS IN PRODUCTION USE!  PLEASE READ EACH STEP CAREFULLY!

In order to log into MariaDB to secure it, we'll need the current
password for the root user.  If you've just installed MariaDB, and
you haven't set the root password yet, the password will be blank,
so you should just press enter here.

Enter current password for root (enter for none): 
OK, successfully used password, moving on...

Setting the root password ensures that nobody can log into the MariaDB
root user without the proper authorisation.

Set root password? [Y/n] y
New password: 
Re-enter new password: 
Password updated successfully!
Reloading privilege tables..
 ... Success!


By default, a MariaDB installation has an anonymous user, allowing anyone
to log into MariaDB without having to have a user account created for
them.  This is intended only for testing, and to make the installation
go a bit smoother.  You should remove them before moving into a
production environment.

Remove anonymous users? [Y/n] y
 ... Success!

Normally, root should only be allowed to connect from 'localhost'.  This
ensures that someone cannot guess at the root password from the network.

Disallow root login remotely? [Y/n] n
 ... skipping.
 By default, MariaDB comes with a database named 'test' that anyone can
access.  This is also intended only for testing, and should be removed
before moving into a production environment.
Remove test database and access to it? [Y/n] y
 - Dropping test database...
 ... Success!
 - Removing privileges on test database...
 ... Success!
Reloading the privilege tables will ensure that all changes made so far
will take effect immediately.
Reload privilege tables now? [Y/n] y
 ... Success!
Cleaning up...
All done!  If you've completed all of the above steps, your MariaDB
installation should now be secure.
Thanks for using MariaDB!

MariaDB [(none)]> SHOW SLAVE STATUS\G;
*************************** 1. row ***************************
               Slave_IO_State: Waiting for master to send event
                  Master_Host: 10.128.0.2
                  Master_User: hinotamashi
                  Master_Port: 3306
                Connect_Retry: 60
              Master_Log_File: mysql_binary_log.000008
          Read_Master_Log_Pos: 474
               Relay_Log_File: mariadb-relay-bin.000002
                Relay_Log_Pos: 536
        Relay_Master_Log_File: mysql_binary_log.000008
             Slave_IO_Running: Yes
            Slave_SQL_Running: Yes
              Replicate_Do_DB: 
          Replicate_Ignore_DB: 
           Replicate_Do_Table: 
       Replicate_Ignore_Table: 
      Replicate_Wild_Do_Table: 
  Replicate_Wild_Ignore_Table: 
                   Last_Errno: 0
                   Last_Error: 
                 Skip_Counter: 0
          Exec_Master_Log_Pos: 474
              Relay_Log_Space: 832
              Until_Condition: None
               Until_Log_File: 
                Until_Log_Pos: 0
           Master_SSL_Allowed: No
           Master_SSL_CA_File: 
           Master_SSL_CA_Path: 
              Master_SSL_Cert: 
            Master_SSL_Cipher: 
               Master_SSL_Key: 
        Seconds_Behind_Master: 0
Master_SSL_Verify_Server_Cert: No
                Last_IO_Errno: 0
                Last_IO_Error: 
               Last_SQL_Errno: 0
               Last_SQL_Error: 
  Replicate_Ignore_Server_Ids: 
			 Master_Server_Id: 1
1 row in set (0.00 sec)
ERROR: No query specified
