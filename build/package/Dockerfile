FROM golang:1.8-alpine
ADD ./gospace/ /go/src/coop
RUN go install coop

FROM alpine:latest
COPY ./web/ /web/
COPY --from=0 /go/bin/coop .
ENV PORT 8080
CMD ["./coop"]
