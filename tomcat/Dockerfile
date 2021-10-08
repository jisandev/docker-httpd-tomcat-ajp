FROM tomcat:9.0.52-jre8-openjdk
# Enable manager
RUN rm -r /usr/local/tomcat/webapps
RUN mv /usr/local/tomcat/webapps.dist /usr/local/tomcat/webapps
COPY ./manager_context.xml /usr/local/tomcat/webapps/manager/META-INF/context.xml
# Add users
COPY ./tomcat-users.xml /usr/local/tomcat/conf/tomcat-users.xml
# Setting
COPY ./server.xml /usr/local/tomcat/conf/
# Expose ports and run 
EXPOSE 8005
EXPOSE 8009
EXPOSE 8080
EXPOSE 8443
CMD ["catalina.sh", "run"]