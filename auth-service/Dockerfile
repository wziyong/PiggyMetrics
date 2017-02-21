FROM piggymetrics_pinpoint
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/auth-service.jar /app/

CMD java -Xmx200m -javaagent:/pinpoint/pinpoint-bootstrap-1.6.0-SNAPSHOT.jar -Dpinpoint.agentId=110002 -Dpinpoint.applicationName=auth-service -jar /app/auth-service.jar >> /var/xx.log


EXPOSE 5000