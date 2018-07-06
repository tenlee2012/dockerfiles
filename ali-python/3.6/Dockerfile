FROM ubuntu:18.04
ENV py_version=3.6.6
RUN sed -i 's/archive.ubuntu.com/mirrors.aliyun.com/g' /etc/apt/sources.list \
    && apt-get update \
    && apt-get install -y python3.6-distutils python3-pip cron vim\
    && ln -s /usr/bin/python3.6 /usr/bin/python \
    && ln -s /usr/bin/pip3 /usr/bin/pip \
    && apt-get clean \
    && apt-get autoclean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*  \
CMD ["bash"]
