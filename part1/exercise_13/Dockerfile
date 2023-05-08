# Dockerfile for starting the example-backend

# Install Golang version 1.16 
FROM golang:1.16

# expose port 
EXPOSE 8080

WORKDIR /usr/src/app

# Copy all source code
COPY . . 

# build the project, will generate binary named "server"
RUN go build

# add environment variables
# ENV REQUEST_ORIGIN="http://localhost:8080"
ENV REQUEST_ORIGIN="http://localhost:3000"

CMD ["./server"]