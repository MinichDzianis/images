ARG ENV_SOURCE_IMAGE
ARG PHP_VERSION
FROM ${ENV_SOURCE_IMAGE}:${PHP_VERSION}
USER root

RUN npm install -g grunt-cli gulp yarn @bitrix/cli

USER www-data
