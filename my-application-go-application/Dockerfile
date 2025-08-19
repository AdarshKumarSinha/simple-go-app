# Base Image
FROM golang:latest

# Set the Current Working Directory inside the container
WORKDIR /app

# Copy everything from the current directory to the container
COPY . .

# Download dependencies
RUN go mod download

# Build the Go app
RUN go build -o main .

# Expose port 8080
EXPOSE 8080

# Command to run the executable
CMD ["./main"]
