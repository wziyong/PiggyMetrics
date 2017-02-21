FROM java:8-jre
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/account-service.jar /app/

ADD ../pinpoint/pinpoint-agent-1.6.0-SNAPSHOT/ /pinpoint/

CMD ["java", "-Xmx200m", "-jar", "/app/account-service.jar","-javaagent:/pinpoint/pinpoint-bootstrap-1.6.0-SNAPSHOT.jar -Dpinpoint.agentId=100001 -Dpinpoint.applicationName=account-service"]

EXPOSE 6000