# NAME:   shebgregor/ubuntu-cpp-psql
FROM partlab/ubuntu-postgresql

LABEL maintainer "Michael Popsuev <sheb.gregor@gmail.com>"

RUN true \
 && apt-get update \
 && apt-get install -y \
	git \
	build-essential \
	pkg-config \
	autoconf \
	automake \
	libtool \
	bison \
	flex \
	libpq-dev \
	libboost-all-dev\
	gcc \
	g++ \
	cpp \
	postgresql-client 
