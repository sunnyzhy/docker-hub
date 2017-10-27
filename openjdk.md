# Docker Pull Command
``` javascript
# docker pull openjdk
```

# Dockerfile
``` bash
FROM openjdk

ADD src.jar /usr/local/java/dest.jar

EXPOSE <container port>

ENTRYPOINT ["java","-jar","/usr/local/java/dest.jar"]
```

# build & run
``` javascript
# docker build -t zhy/java-jar .

# docker run -p <host port>:<container port> --name running-jar zhy/java-jar
```