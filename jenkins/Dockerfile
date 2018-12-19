FROM java:8u111-jdk
#定义时区参数
ENV TZ=Asia/Beijing
#设置时区
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo '$TZ' > /etc/timezone

RUN mkdir -p /usr/src/app && mkdir -p /data/jenkinstest

WORKDIR /usr/src/app

COPY target/jenkins-0.0.1-SNAPSHOT.jar /usr/src/app

CMD java -jar jenkins-0.0.1-SNAPSHOT.jar