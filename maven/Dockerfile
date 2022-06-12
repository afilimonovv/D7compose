FROM maven:3.6-alpine
WORKDIR /tmp/
CMD ["apk update \
    && apk add git \
    && git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git git \
    && mvn -f /git/pom.xml package \
    && cp ./git/target/*.war /tmp"]




#CMD ["/bin/bash", "-c", "apk update \
#    && apk add git \
#   && git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git git \
#    && mvn -f /git/pom.xml package \
#    && cp ./git/target/*.war /war"]