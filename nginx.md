# Docker Pull Command
``` bash
# docker pull nginx
```

# Dockerfile
``` bash
FROM nginx

COPY static-html-directory /usr/share/nginx/html

COPY nginx.conf /etc/nginx/nginx.conf
```