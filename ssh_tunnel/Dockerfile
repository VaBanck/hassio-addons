FROM ghcr.io/home-assistant/base:latest

RUN apk add --no-cache openssh

RUN ssh-keygen -b 2048 -t rsa -f /root/.ssh/id_rsa -q -N ""

COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]