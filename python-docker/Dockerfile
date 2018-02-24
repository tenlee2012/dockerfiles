FROM debian:stretch
MAINTAINER tenlee <tenlee2012@gmail.com>

RUN apt-get update && \
	apt-get install --assume-yes --no-install-recommends \
	gcc libffi-dev libssl-dev libxml2-dev libxslt1-dev \
	python3-dev python3-pip zlib1g-dev && \
	apt-get clean && \
	rm -rf /var/cache/apt/archives/* /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
	ln -s pip3 /usr/bin/pip && \
	ln -s python3 /usr/bin/python && \
	pip install --upgrade pip && \
	pip install --upgrade setuptools wheel
