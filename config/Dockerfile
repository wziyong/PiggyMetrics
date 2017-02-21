FROM piggymetrics_pinpoint
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/config.jar /app/

CMD java -Xmx200m -javaagent:/pinpoint/pinpoint-bootstrap-1.6.0-SNAPSHOT.jar -Dpinpoint.agentId=110003 -Dpinpoint.applicationName=config-service -jar /app/config-service.jar >> /var/xx.log


EXPOSE 8888