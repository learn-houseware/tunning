``wget http://download.jboss.org/wildfly/12.0.0.Final/wildfly-12.0.0.Final.zip ``


###Initialize Wildfly  
``init.sh``

###Start  
``start.sh``

###Java Mission Control 
``jmc.sh``


``wget -qx "http://search.maven.org/remotecontent?filepath=mysql/mysql-\
  connector-java/5.1.39/mysql-connector-java-5.1.39.jar" -O mysql-connector-java.jar`` 
``
###Timeout Attribute
``cli.sh  "/subsystem=transactions/:write-attribute(name=default-timeout,value=6000)"
``
###Timeout Attribute
``cli.sh  "/subsystem=transactions/:write-attribute(name=default-timeout,value=6000)"
``
###Undeploy 
``cli.sh  "undeploy 03-wildfly-1.0-SNAPSHOT"
``

###Wilfly 12 flags
``-Xmx4g
  -XX:+UseG1GC
  -XX:+UnlockCommercialFeatures
  -XX:+FlightRecorder
  -server
  -XX:MetaspaceSize=96M
  -XX:MaxMetaspaceSize=256m
  -Djava.net.preferIPv4Stack=true
  -Djboss.modules.system.pkgs=org.jboss.byteman
  -Djava.awt.headless=true
  -Djboss.bind.address.management=0.0.0.0
  -Duser.timezone=Europe/Madrid
  -Duser.language=es
  -Duser.country=ES``
