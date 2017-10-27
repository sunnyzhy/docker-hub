# Docker Pull Command
``` javascript
# docker pull tomcat
```

# Dockerfile
``` bash
FROM tomcat

COPY web-directory /usr/local/tomcat/webapps/web-directory

EXPOSE 8080
```

# build & run
``` javascript
# docker build -t some-content-tomcat .

# docker run -p 8080:8080 -d --name some-tomcat some-content-tomcat
```
Then you can hit http://localhost:8080/web-directory or http://host-ip:8080/web-directory in your browser.