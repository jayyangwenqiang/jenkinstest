FROM java:8u111-jdk

RUN mkdir -p /usr/src/app && mkdir -p /data/jenkinstest

WORKDIR /usr/src/app

COPY target/jenkins-0.0.1-SNAPSHOT.jar /usr/src/app

CMD java -jar jenkins-0.0.1-SNAPSHOT.jar