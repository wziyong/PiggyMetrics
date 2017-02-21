FROM piggymetrics_pinpoint
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/notification-service.jar /app/

CMD java -Xmx200m -javaagent:/pinpoint/pinpoint-bootstrap-1.6.0-SNAPSHOT.jar -Dpinpoint.agentId=110006 -Dpinpoint.applicationName=notification-service -jar /app/notification-service.jar >> /var/xx.log


EXPOSE 8000