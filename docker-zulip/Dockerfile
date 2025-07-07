FROM zulip/docker-zulip:10.4-0

ARG RENDER_EXTERNAL_HOSTNAME
ENV SETTING_EXTERNAL_HOST=${SETTING_EXTERNAL_HOST:-$RENDER_EXTERNAL_HOSTNAME}
RUN apt-get update && apt-get install -y nano python3-dev
RUN chown zulip:zulip /usr/bin/supervisorctl

CMD ["/usr/bin/supervisord"]
USER root
