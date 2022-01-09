FROM openjdk:11

COPY install-synthea.sh /tmp/install-synthea.sh
RUN bash /tmp/install-synthea.sh

RUN apt-get update && apt-get install jq -y

COPY run-synthea.sh /tmp/run-synthea.sh
COPY entry.sh /entry.sh
ENTRYPOINT [ "bash", "/entry.sh" ]
 