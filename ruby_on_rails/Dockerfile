FROM ubuntu:14.04
Maintainer Daniel Klopp
# Thank you https://gorails.com/setup/ubuntu/14.04
# Thank you famelis at https://github.com/phusion/baseimage-docker/issues/58
RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections
RUN apt-get update
RUN apt-get -y upgrade
RUN apt-get -y install ssh whois nano git
RUN apt-get -y install man-db gdb
RUN apt-get -y install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties
RUN apt-get -y install libgdbm-dev libncurses5-dev automake libtool bison libffi-dev
RUN apt-get -y install curl
RUN curl -L -o rvm.sh https://get.rvm.io
RUN bash rvm.sh stable 
RUN rm -f rvm.sh
RUN source /etc/profile.d/rvm.sh
#RUN echo "source /etc/profile.d/rvm.sh" >> ~/.bashrc
RUN rvm install 2.1.2
RUN rvm use 2.1.2 --default
