FROM centos:centos6
Maintainer Daniel Klopp
RUN yum -y update
RUN yum -y install redhat-lsb-core wget
#RUN wget https://opscode-omnibus-packages.s3.amazonaws.com/el/6/x86_64/chef-server-11.1.4-1.el6.x86_64.rpm
#RUN rpm -ivh ./chef-server-11.1.4-1.el6.x86_64.rpm
RUN mv /sbin/initctl /sbin/initctl.orig
RUN ln -s /bin/true /sbin/initctl
#RUN chef-server-ctl reconfigure

#EXPOSE 443
