FROM wzy/pinpoint
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/account-service.jar /app/

CMD ["java", "-Xmx200m", "-jar", "/app/account-service.jar","-javaagent:/pinpoint/pinpoint-bootstrap-1.6.0-SNAPSHOT.jar -Dpinpoint.agentId=100001 -Dpinpoint.applicationName=account-service"]

EXPOSE 6000