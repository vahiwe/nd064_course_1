# Get base Image
FROM golang:alpine

# Set Working directory
WORKDIR /go/src/app

# Add Source code into image
ADD . /go/src/app

# Initialize go modules
RUN go mod init

# Build Binary of source code
RUN go build -o helloworld

# Expose port 6111
EXPOSE 6111

# Run Binary
CMD ["./helloworld"]