#FROM sergeyzh/centos6-epel
FROM ubuntu:12.04
Maintainer Daniel Klopp
RUN apt-get update
RUN apt-get -y upgrade
RUN apt-get -y install wget
RUN wget --no-check-certificate https://opscode-omnibus-packages.s3.amazonaws.com/ubuntu/12.04/x86_64/chef-server_11.1.4-1_amd64.deb
RUN dpkg -i ./chef-server_11.1.4-1_amd64.deb
RUN chef-server-ctl reconfigure

