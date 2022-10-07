FROM golang:1.15.6-alpine

LABEL maintainer="Ankit Kumar <ankitkumar0000333@gmail.com>"

WORKDIR $GOPATH/src/github.com/Ankit0003/SellerApp-Project/collector-api

COPY . .

RUN go get -d -v ./...

RUN go install -v ./...

EXPOSE 8081

CMD ["collector-api"]