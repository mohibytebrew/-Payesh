FROM tomcat:9-jdk11

ADD https://jdbc.postgresql.org/download/postgresql-42.7.3.jar \
    /usr/local/tomcat/lib/

COPY gse/GitaServerEngine /usr/local/tomcat/webapps/GitaServerEngine

EXPOSE 8080

CMD ["catalina.sh", "run"]

