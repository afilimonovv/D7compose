FROM maven:3.6-alpine
RUN apk update
RUN apk add git
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR boxfuse-sample-java-war-hello/
RUN mvn package
CMD ["cp", "/boxfuse-sample-java-war-hello/target/hello-1.0.war", "/war"]


