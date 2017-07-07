FROM debian:7.10

RUN echo "deb http://mirrors.aliyun.com/debian/ wheezy main non-free contrib" > /etc/apt/sources.list && \
echo "deb http://mirrors.aliyun.com/debian/ wheezy-proposed-updates main non-free contrib" >> /etc/apt/sources.list && \
echo "deb-src http://mirrors.aliyun.com/debian/ wheezy main non-free contrib" >> /etc/apt/sources.list && \
echo "deb-src http://mirrors.aliyun.com/debian/ wheezy-proposed-updates main non-free contrib" >> /etc/apt/sources.list && \
echo "deb http://mirrors.163.com/debian/ wheezy-backports main non-free contrib" >> /etc/apt/sources.list && \
echo "deb-src http://mirrors.163.com/debian/ wheezy-backports main non-free contrib" >> /etc/apt/sources.list && \
cat /etc/apt/sources.list && \
apt-get update && \
    apt-get install -y --no-install-recommends \
        build-essential \
        libsasl2-dev \
        libldap2-dev \
        libc-dev \
        g++ \
        mysql-client-5.5 \
        curl \
        libfreetype6-dev \
        libpng12-dev \
        libzmq3-dev \
        pkg-config \
        python \
        python-dev \
        rsync \
        software-properties-common \
        unzip \
        vim-nox \
        wget \
        strace \
        sudo \
        tmux \
        net-tools \
        procps \
        graphviz \
        libmysqlclient-dev \
        git \
        && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*


RUN curl -O --insecure https://raw.githubusercontent.com/pypa/get-pip/master/get-pip.py && \
    python get-pip.py && \
    rm get-pip.py
