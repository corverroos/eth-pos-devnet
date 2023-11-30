# This dockerfile builds and runs the golang logproxy application
FROM golang:alpine

# Copy the main.go into the container
WORKDIR /app
COPY go.* .
COPY main.go .

# Install the logproxy
RUN go install .

# Run the logproxy
CMD ["logproxy"]

