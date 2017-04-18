# ###############################################################################
# Base image
################################################################################

FROM ubuntu:16.04

################################################################################
# Build instructions
################################################################################

RUN mkdir -p /var/www/default

COPY ./deploy /var/www/default

RUN find /var/www/default/. -type d -exec chmod 775 {} \;
RUN find /var/www/default/. -type d -exec chmod 775 {} \;
RUN find /var/www/default/. -type f -exec chmod 664 {} \;
RUN chown -R www-data:www-data /var/www/default/*
