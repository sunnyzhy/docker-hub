# Docker Pull Command
``` javascript
# docker pull nginx
```

# Dockerfile
``` bash
FROM nginx

COPY static-html-directory /usr/share/nginx/html

COPY nginx.conf /etc/nginx/nginx.conf
```

# build & run
``` javascript
# docker build -t some-content-nginx .

# docker run -d --name some-nginx some-content-nginx
```
Then you can hit http://localhost/static-html-directory or http://host-ip/static-html-directory in your browser.