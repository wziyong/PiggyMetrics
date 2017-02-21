FROM wzy/pinpoint
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/account-service.jar /app/

CMD java -Xmx200m -javaagent:/pinpoint/pinpoint-bootstrap-1.6.0-SNAPSHOT.jar -Dpinpoint.agentId=110001 -Dpinpoint.applicationName=account-service -jar /app/account-service.jar >> /var/xx.log

EXPOSE 6000