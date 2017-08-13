# Pull base image
FROM nginx:1.10

MAINTAINER Serghei Iakovlev <serghei@phalconphp.com>

ENV PROVISION_CONTEXT "development"

# Deploy scripts/configurations
COPY bin/*.sh /opt/docker/provision/entrypoint.d/

RUN \
    # Custom provisions
    chmod +x /opt/docker/provision/entrypoint.d/*.sh \
