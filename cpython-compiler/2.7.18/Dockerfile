FROM python:2.7.18

RUN apt update
RUN apt upgrade -y

RUN apt install -y gcc debhelper\
        cdbs\
        lintian\
        build-essential\
        fakeroot \
        devscripts\
        pbuilder \
        dh-make\
        debootstrap\ 
        python-pip

WORKDIR /code/

ENTRYPOINT ["/bin/bash"]
