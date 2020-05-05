FROM centos:centos7

RUN yum -y update && yum clean all
RUN yum install -y which wget tar vim emacs openssh-server openssh-clients

RUN mkdir  ~/.ssh
RUN touch  ~/.ssh/authorized_keys
RUN chmod 600  ~/.ssh/authorized_keys

CMD /sbin/init
