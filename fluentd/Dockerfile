FROM fluent/fluentd:v1.7-1

# Use root account to use apk
USER root

# below RUN includes plugin as examples elasticsearch is not required
# you may customize including plugins as you wish
RUN sudo gem install fluent-plugin-elasticsearch \
 && sudo gem install fluent-plugin-grok-parser 

COPY fluent.conf /fluentd/etc/
ENV FLUENTD_CONF="fluent.conf"
