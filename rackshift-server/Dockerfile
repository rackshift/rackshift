FROM rackshift/rackshift-base:1.0

RUN mkdir -p /opt/rackshift

ADD ./target/rackshift-server-1.0.0.jar /opt

VOLUME /opt/rackshift

EXPOSE 5005

CMD java -jar -Xdebug -Xrunjdwp:transport=dt_socket,address=5005,server=y,suspend=n /opt/rackshift-server-1.0.0.jar