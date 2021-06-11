FROM golang:alpine

WORKDIR /go/src/app

ADD . .

RUN ["go", "mod", "init", "main"]

RUN ["go", "mod", "tidy"]

RUN ["go", "build", "-o", "helloworld"]

EXPOSE 6111

CMD ["./helloworld"]
