# WS Lundstrom - tomcat
mvn initialize && mvn compile && mvn package
rm -rf /opt/apache-tomcat-VERSION/webapps/ws-lundstrom /opt/apache-tomcat-VERSION/webapps/ws-lundstrom.war 
mv target/ws-lundstrom target/ws-lundstrom.war /opt/apache-tomcat-VERSION/webapps/ 
/opt/apache-tomcat-VERSION/bin/shutdown.sh 
/opt/apache-tomcat-VERSION/bin/catalina.sh 
