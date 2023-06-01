FROM zulip/docker-zulip:latest

ARG RENDER_EXTERNAL_HOSTNAME
ENV SETTING_EXTERNAL_HOST=${SETTING_EXTERNAL_HOST:-$RENDER_EXTERNAL_HOSTNAME}
RUN apt-get update && apt-get install -y nano python-dev

EXPOSE 80 443
ENTRYPOINT ["/sbin/entrypoint.sh"]
