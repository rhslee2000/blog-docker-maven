FROM frolvlad/alpine-oraclejdk8:slim
MAINTAINER Raymond Lee <raymond.lee@gmail.com>
VOLUME /tmp
ADD docker-maven-IMAGE_VERSION.jar app.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]
