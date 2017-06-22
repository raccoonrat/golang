FROM scratch
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
ENV http_proxy=http://cn-proxy.jp.oracle.com:80
ENV https_proxy=http://cn-proxy.jp.oracle.com:80
ADD oraclelinux-7.3-rootfs.tar.xz /
RUN yum --enablerepo=ol7_addons update && yum install -y curl && yum install -y wget
# RUN curl -sSL https://get.docker.com/ | sh
# overwrite this with 'CMD []' in a dependent Dockerfile
CMD ["/bin/bash"]
