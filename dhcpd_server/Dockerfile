FROM ubuntu:14.04
Maintainer Daniel Klopp
# Thank you famelis at https://github.com/phusion/baseimage-docker/issues/58
RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections
RUN apt-get update
RUN apt-get -y upgrade
RUN apt-get -y install ssh whois nano 
RUN apt-get -y install man-db curl wget
RUN apt-get -y install curl tcpdump
RUN apt-get -y install dhcp3-server

