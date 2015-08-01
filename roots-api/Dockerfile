FROM tukiyo3/centos-ja:6.5
MAINTAINER nyoko708

# set locale
RUN yum update -y
RUN yum reinstall -y glibc-common
ENV LANG ja_JP.UTF-8
ENV LANGUAGE ja_JP:ja
ENV LC_ALL ja_JP.UTF-8

# set php
RUN yum vim -y
RUN rpm -Uvh http://ftp.iij.ad.jp/pub/linux/fedora/epel/6/x86_64/epel-release-6-8.noarch.rpm
RUN rpm -Uvh http://rpms.famillecollet.com/enterprise/remi-release-6.rpm
RUN yum install --enablerepo=remi --enablerepo=remi-php56 php -y
RUN yum --enablerepo=epel install libmcrypt -y
RUN yum --enablerepo=epel install php-mcrypt -y
