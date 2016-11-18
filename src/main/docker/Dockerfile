FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD pipelinespringbootdemo-0.0.1-SNAPSHOT.jar pipelinespringbootdemo-0.0.1-SNAPSHOT.jar
RUN sh -c 'touch /pipelinespringbootdemo-0.0.1-SNAPSHOT.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /pipelinespringbootdemo-0.0.1-SNAPSHOT.jar" ]