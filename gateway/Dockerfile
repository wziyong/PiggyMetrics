FROM java:8-jre
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/gateway.jar /app/

CMD java -Xmx200m -javaagent:/pinpoint/pinpoint-bootstrap-1.6.0-SNAPSHOT.jar -Dpinpoint.agentId=110004 -Dpinpoint.applicationName=gateway-service -jar /app/gateway.jar >> /var/xx.log


EXPOSE 4000