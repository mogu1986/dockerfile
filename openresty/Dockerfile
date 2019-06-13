FROM openresty/openresty:1.13.6.2-centos
MAINTAINER gaowei <gaowei@fengjinggroup.com>

RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && echo 'Asia/Shanghai' >/etc/timezone

RUN rm -rf /etc/nginx/conf.d/*