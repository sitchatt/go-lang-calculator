###########################################
# BASE IMAGE
###########################################

FROM ubuntu

RUN apt-get update && apt install golang-go

ENV GO111MODULE=off

COPY . .

RUN CGO_ENABLED=0 go build -o /app .

ENTRYPOINT ["/app"]

