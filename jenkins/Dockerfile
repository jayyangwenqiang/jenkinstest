FROM java:8u111-jdk

RUN apt-get install tzdata \
    && rm /etc/localtime \
    && ln -s /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && mkdir -p /usr/src/app \ 
    && mkdir -p /data/jenkinstest \
    && echo "Asia/Shanghai" > /etc/timezone

WORKDIR /usr/src/app

COPY target/jenkins-0.0.1-SNAPSHOT.jar /usr/src/app

CMD java -jar jenkins-0.0.1-SNAPSHOT.jar