FROM java:8

ENV SPRING_ACTIVE_PROFILES docker

ADD app.jar app.jar

RUN bash -c 'touch /app.jar'

EXPOSE 8989

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
