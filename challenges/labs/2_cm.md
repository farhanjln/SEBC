[root@instance-2 hinotamashi94]# ls /etc/yum.repos.d/
CentOS-Base.repo       CentOS-fasttrack.repo  CentOS-Vault.repo      mysql-community.repo
CentOS-CR.repo         CentOS-Media.repo      cloudera-manager.repo  mysql-community-source.repo
CentOS-Debuginfo.repo  CentOS-Sources.repo    google-cloud.repo

root@instance-2 hinotamashi94]# /usr/share/cmf/schema/scm_prepare_database.sh -h 10.128.0.2 mysql scm scm
Enter SCM password: 
JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/java/jdk1.7.0_67-cloudera/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java
/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/
cloudera-scm-server/db.properties com.cloudera.cmf.db.
[                          main] DbCommandExecutor              INFO  Successfully connected to database.
All done, your SCM database is configured correctly!
[root@instance-2 hinotamashi94]# 
