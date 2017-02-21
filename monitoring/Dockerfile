FROM piggymetrics_pinpoint
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/monitoring.jar /app/

CMD java -Xmx200m -javaagent:/pinpoint/pinpoint-bootstrap-1.6.0-SNAPSHOT.jar -Dpinpoint.agentId=110005 -Dpinpoint.applicationName=monitoring-service -jar /app/monitoring-service.jar >> /var/xx.log


EXPOSE 8989 8080