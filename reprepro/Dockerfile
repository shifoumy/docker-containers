FROM debian

RUN apt update
RUN apt upgrade -y
RUN apt install -y reprepro vim apt-transport-https ca-certificates \
    curl\
    gnupg-agent\
    software-properties-common\
    lsb-release\
    wget

entrypoint ["/bin/bash"]
