FROM golang

LABEL maintainer "student@heptio.com"
LABEL gowebapp "v1"

EXPOSE 80

ENV GOPATH=/go
ENV DB_PASSWORD=heptio
COPY /code $GOPATH/src/gowebapp
WORKDIR $GOPATH/src/gowebapp/
RUN go get && go install

VOLUME $GOPATH/src/gowebapp/config

ENTRYPOINT $GOPATH/bin/gowebapp 
