FROM mysql:5.6

LABEL maintainer "education@heptio.com"
LABEL gowebapp-mysql "v1"

COPY gowebapp.sql /docker-entrypoint-initdb.d/

