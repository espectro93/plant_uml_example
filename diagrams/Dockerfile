FROM ubuntu:latest
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y \
    default-jre-headless
RUN apt-get install -y plantuml
RUN apt-get clean
WORKDIR /app
COPY . /app
RUN chmod -R 777 /app
ENTRYPOINT ["plantuml"]
