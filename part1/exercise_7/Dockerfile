# Start from the ubuntu image
FROM ubuntu:20.04

# Install curl into image
RUN apt-get update 
RUN apt-get install -y curl

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the find.sh file from this location to /usr/src/app/ creating /usr/src/app/find.sh
COPY find.sh .

# Add execution permissions during the build.
RUN chmod +x find.sh

# When running docker run the command will be ./find.sh
CMD ./find.sh