FROM centos

RUN useradd admin

RUN ["echo", "altkom", "|", "passwd", "--stdin", "admin"]
RUN sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-*
RUN sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-*

RUN yum -y update && yum -y install cifs-utils

CMD ["tail -f /dev/null"]
