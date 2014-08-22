FROM sergeyzh/centos6-epel
Maintainer Daniel Klopp
RUN yum -y update
RUN
RUN apt-get -y upgrade
RUN wget https://opscode-omnibus-packages.s3.amazonaws.com/el/6/x86_64/chef-server-11.1.4-1.el6.x86_64.rpm
RUN rpm -ivh ./chef-server-11.1.4-1.el6.x86_64.rpm
RUN chef-server-ctl reconfigure

EXPOSE 443
