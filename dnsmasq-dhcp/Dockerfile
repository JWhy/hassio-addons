#ARG BUILD_FROM
#FROM $BUILD_FROM
FROM homeassistant/aarch64-base:latest

# Add env
ENV LANG C.UTF-8

# Setup base
RUN apk add --no-cache dnsmasq

# Copy data
COPY run.sh /
COPY dnsmasq.conf /etc/

CMD [ "/run.sh" ]
