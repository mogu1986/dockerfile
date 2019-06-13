FROM java:8-jdk-alpine
MAINTAINER gaowei@fengjinggroup.com
ENV TZ Asia/Shanghai
ENV JAVA_OPS="-Duser.timezone=Asia/Shanghai"
EXPOSE 8080
RUN apk add --no-cache tzdata \
&& echo "Asiz/Shanghai" > /etc/timezone \
&& ln -sf /usr/share/zoneinfo/Asiz/Shanghai /etc/localtime