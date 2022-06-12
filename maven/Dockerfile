/bin/bash -c "apk update \
      && apk add git \
      && git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git git \
      && mvn -f /git/pom.xml package \
      && cp ./git/target/*.war /war"