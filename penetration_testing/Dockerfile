FROM ubuntu:14.04
Maintainer Daniel Klopp
RUN apt-get update
RUN apt-get -y install ssh
RUN apt-get -y install whois
RUN apt-get -y install nano
RUN apt-get -y install git
RUN apt-get -y install dnsutils
RUN apt-get -y install man-db
RUN apt-get -y install wget
RUN wget https://dnsmap.googlecode.com/files/dnsmap-0.30.tar.gz
RUN tar -xf dnsmap-0.30.tar.gz
RUN apt-get -y install build-essential
RUN make -C /dnsmap-0.30
RUN cp /dnsmap-0.30/dnsmap /usr/bin
RUN apt-get -y install gdb

