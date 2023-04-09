# We need ruby 3.1.0. I found this from Docker Hub
FROM golang:1.16

EXPOSE 8080
WORKDIR /usr/src/app
COPY ./app .

# Compile by following instructions from README
ENV REQUEST_ORIGIN http://localhost:5050
RUN go build
CMD ["./server"]