FROM tomcat:8-jdk11
MAINTAINER yejisoft@gmail.com

COPY ./ROOT.war /usr/local/tomcat/webapps/staging.war
RUN ["mkdir", "/hamonize"]
COPY ./environment.txt /hamonize/environment.txt

CMD ["catalina.sh","run"]

RUN ["mv", "/usr/local/tomcat/webapps/staging.war","/usr/local/tomcat/webapps/ROOT.war"]
RUN ["rm", "-rf", "/usr/local/tomcat/webapps/ROOT"]
