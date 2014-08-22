#FROM sergeyzh/centos6-epel
# This one won't work as Ubuntu's upstart and package management are not
# well supported with vmware https://github.com/docker/docker/issues/1024
FROM ubuntu:12.04
Maintainer Daniel Klopp
RUN apt-get update
RUN apt-get -y upgrade
RUN apt-get -y install wget vim nano less
RUN wget --no-check-certificate https://opscode-omnibus-packages.s3.amazonaws.com/ubuntu/12.04/x86_64/chef-server_11.1.4-1_amd64.deb
RUN dpkg -i ./chef-server_11.1.4-1_amd64.deb

RUN chef-server-ctl reconfigure

EXPOSE 443
