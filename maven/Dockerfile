FROM maven:3.6-alpine
RUN mkdir -p /war/
WORKDIR /war/
RUN apk update
RUN apk add git
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git git
#CMD ["mvn",  "package" ]
RUN mvn -f /git/pom.xml package
RUN cp ./git/target/*.war /war/"]



#CMD ["mvn", "package"]
# RUN cp ./git/target/*.war ./war




#CMD ["/bin/bash", "-c", "apk update \
#    && apk add git \
#   && git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git git \
#    && mvn -f /git/pom.xml package \
#    && cp ./git/target/*.war /war"]