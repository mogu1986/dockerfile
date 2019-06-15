FROM williamyeh/ansible:centos7
MAINTAINER gaowei <gaowei@fengjinggroup.com>
RUN yum install -y kde-l10n-Chinese
ENV LANG="zh_CN.UTF-8"
ADD ansible.cfg /etc/ansible/ansible.cfg
ADD locale.conf /etc/locale.conf