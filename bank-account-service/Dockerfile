
FROM openjdk:8-jre-alpine

MAINTAINER Brian Hannaway

WORKDIR /app

# Add wait script to the image - script pulled from https://github.com/ufoscout/docker-compose-wait/releases/download/2.7.3/wait /wait
COPY /scripts/wait /app/
RUN chmod -R +x /app
RUN ls -lrth /app

RUN apk --no-cache add curl

COPY /target/bank-account-service-0.0.1-SNAPSHOT.jar /app/

CMD ./wait && java -jar bank-account-service-0.0.1-SNAPSHOT.jar