FROM centos:centos6
Maintainer Daniel Klopp
RUN yum -y update
RUN yum -y install redhat-lsb-core wget
RUN mv /sbin/initctl /sbin/initctl.orig
RUN ln -s /bin/true /sbin/initctl
RUN rpm -ivh http://mirror.utexas.edu/epel/6/i386/epel-release-6-8.noarch.rpm
RUN yum -y install couchdb
RUN service couchdb start
RUN chkconfig --level 345 couchdb on
RUN yum -y install rabbitmq-server
RUN service rabbitmq-server start
RUN chkconfig --level 345 rabbitmq-server on
RUN rabbitmqctl add_vhost /chef
RUN rabbitmqctl add_user chef testing
RUN rabbitmqctl set_permissions -p /chef chef ".*" ".*" ".*"

RUN yum -y install gecode
#RUN chef-server-ctl reconfigure

#EXPOSE 443
