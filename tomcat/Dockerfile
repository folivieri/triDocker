FROM tomcat:7

MAINTAINER fred.olivieri@gmail.com

# add context to /usr/local/tomcat/webapps

ENV TZ=America/Los_Angeles
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

#COPY TriNet.xml /usr/local/tomcat/conf/Catalina/localhost/TriNet.xml

#COPY trinetGateway.xml /usr/local/tomcat/conf/Catalina/localhost/trinetGateway.xml

COPY context.xml /usr/local/tomcat/conf/context.xml

COPY ojdbc6.jar /usr/local/tomcat/lib/ojdbc6.jar

RUN ls -la /usr/local/tomcat/webapps > /tmp/contents.txt

