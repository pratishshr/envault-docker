FROM python:2.7-alpine

# Install ["python3", "nodejs", "yarn", "envault"]
RUN apk add --no-cache python3 && \
  apk add --no-cache --repository http://dl-cdn.alpinelinux.org/alpine/v3.7/main/ nodejs=8.9.3-r1 && \
  npm install -g yarn && \
  pip3 install envault==0.4.5 

# Set environment variables
# ("Click" requires UTF-8 encoding for the environment)
ENV LANG=C.UTF-8
ENV LC_ALL=C.UTF-8 