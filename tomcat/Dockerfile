FROM tomcat:8.0.30-jre8

COPY ./<yourAppName>.war /usr/local/tomcat/webapps/<yourAppName>.war
COPY ./sqljdbc4.jar /usr/local/tomcat/lib/sqljdbc.jar
COPY ./context.xml /usr/local/tomcat/conf/context.xml

EXPOSE 8009
