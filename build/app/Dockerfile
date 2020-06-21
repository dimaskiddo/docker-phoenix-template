FROM dimaskiddo/alpine:elixir-1.10
MAINTAINER Team Name <team@mail.com>

## Set Environment Variables
ENV PHOENIX_VERSION 1.5.3

# Run as Root User
USER root

# Do Some Customization if Needed Here
RUN apk add --no-cache --update \
      inotify-tools \
    && apk add --no-cache --update --virtual .build-dep \
        build-base \
    && mix do local.hex --force, local.rebar --force \
    && echo y | mix archive.install hex phx_new ${PHOENIX_VERSION}

# Run Command
CMD ["tail","-F","/dev/null"]
