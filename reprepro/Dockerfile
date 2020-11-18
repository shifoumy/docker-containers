FROM debian

RUN apt update
RUN apt upgrade -y
RUN apt install -y reprepro vim apt-transport-https ca-certificates \
    curl\
    gnupg-agent\
    software-properties-common\
    lsb-release\
    wget

RUN mkdir -p /var/www/repo
RUN mkdir -p /var/www/repo/conf
RUN mkdir -p /var/www/repo/incomming

entrypoint ["/bin/bash"]
