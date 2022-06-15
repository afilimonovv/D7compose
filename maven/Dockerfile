FROM maven:3.6-alpine
RUN mkdir -p /war/
WORKDIR /war/
RUN apk update
RUN apk add git
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git git
RUN apk add default-jdk
RUN apk add maven
RUN mvn package
CMD ["cp", "./git/target/hello-1.0.war /war/"]



#



#CMD ["/bin/bash", "-c", "apk update \
#    && apk add git \
#   && git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git git \
#    && mvn -f /git/pom.xml package \
#    && cp ./git/target/*.war /war"]