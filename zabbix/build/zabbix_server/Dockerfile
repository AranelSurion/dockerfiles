FROM zabbix/zabbix-server-pgsql:ubuntu-3.2.4
LABEL maintainer "yekta@iamyekta.com"

COPY slack.sh /usr/lib/zabbix/alertscripts/

RUN chown zabbix:zabbix /usr/lib/zabbix/alertscripts/slack.sh

RUN apt-get update && apt-get install -y curl

RUN rm -rf /var/lib/apt/lists/* && apt-get clean
