FROM ubuntu:bionic
LABEL maintainer "Gustavo Muniz do Carmo <gustavo@codeyourinfra.today>"

# Install python3
RUN apt-get update && \
    apt-get install python3 -y && \
    apt-get clean

CMD ["tail", "-f", "/dev/null"]
