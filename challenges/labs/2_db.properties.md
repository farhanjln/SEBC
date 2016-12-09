root@instance-2 hinotamashi94]# head -1  /var/log/cloudera-scm-server/cloudera-scm-server.log 
2016-12-09 02:57:52,803 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfi
le.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.
schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewG
C, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Ve
rsion: 5.9.0 (#249 built by jenkins on 20161006-1801 git: 898a5e032c080e18833dfc58180761f6ef2ea351)
[root@instance-2 hinotamashi94]# 

[root@instance-2 hinotamashi94]# cat /var/log/cloudera-scm-server/cloudera-scm-server.log |grep "Started Jetty server"
2016-12-09 03:04:09,081 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.
[root@instance-2 hinotamashi94]# 
