FROM golang:latest 
RUN mkdir /app 
ADD . /app/ 
WORKDIR /app
RUN go mod init example.com/testdevops
RUN go get -d
RUN go build -o main . 
CMD ["/app/main"]
EXPOSE 80
