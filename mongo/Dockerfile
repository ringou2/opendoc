FROM openjdk:7-jdk-alpine

# Install required packages
RUN apk add --no-cache \
    bash  tzdata busybox-extras;
ENV  TIME_ZONE Asia/Shanghai
RUN  echo "${TIME_ZONE}" > /etc/timezone
RUN  ln -sf /usr/share/zoneinfo/${TIME_ZONE} /etc/localtime 