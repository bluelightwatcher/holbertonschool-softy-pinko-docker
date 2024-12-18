# Use the latest Ubuntu image
FROM ubuntu:latest

# Update APT and upgrade all installed software
RUN apt-get update 
RUN apt-get upgrade -y
RUN apt-get install -y  python3 python3-pip
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install flask flask-cors


# Copy app file into directory
COPY api.py /app/api.py

# Change working directory
WORKDIR /app

# Exposing port
EXPOSE 5252

# Executing command targeting the docker image inside the directory
CMD ["python3", "api.py"]
