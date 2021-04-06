FROM tomcat:9-jre9
MAINTAINER yejisoft@gmail.com

COPY ./ROOT.war /usr/local/tomcat/webapps/staging.war

CMD ["catalina.sh","run"]

RUN ["mv", "/usr/local/tomcat/webapps/staging.war","/usr/local/tomcat/webapps/ROOT.war"]
RUN ["rm", "-rf", "/usr/local/tomcat/webapps/ROOT"]
