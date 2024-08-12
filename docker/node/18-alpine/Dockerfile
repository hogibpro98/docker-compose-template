FROM node:22.6.0-bullseye

ENV USERNAME=www-data
ENV APP_HOME /www

WORKDIR $APP_HOME

# Create document root, fix permissions, and change owner
RUN chown -R ${USERNAME}:${USERNAME} $APP_HOME

COPY start.sh /scripts/start.sh
RUN chmod +x /scripts/start.sh

CMD ["/scripts/start.sh"]

