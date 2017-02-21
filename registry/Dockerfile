FROM piggymetrics_pinpoint
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/registry.jar /app/

CMD java -Xmx200m -javaagent:/pinpoint/pinpoint-bootstrap-1.6.0-SNAPSHOT.jar -Dpinpoint.agentId=110007 -Dpinpoint.applicationName=registry-service -jar /app/registry-service.jar >> /var/xx.log


EXPOSE 8761