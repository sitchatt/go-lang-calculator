###########################################
# BASE IMAGE
###########################################

FROM ubuntu

ENV GO111MODULE=off

COPY . .

RUN CGO_ENABLED=0 go build -o /app .

ENTRYPOINT ["/app"]

