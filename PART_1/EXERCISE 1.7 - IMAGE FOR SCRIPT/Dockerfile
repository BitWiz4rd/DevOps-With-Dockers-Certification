# Start from the alpine image
FROM ubuntu:20.04

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Update apt repos
RUN apt update

# Install curl using apt
RUN apt install -y curl

# Copy the hello.sh file from this location to /usr/src/app/ creating /usr/src/app/hello.sh.
COPY curl.sh .

# When running Docker run the command will be ./hello.sh
CMD ./curl.sh
