FROM dimaskiddo/alpine:elixir-1.10.3
MAINTAINER Team Name <team@mail.com>

# Set Environment Variables
ENV PHOENIX_VERSION 1.5.3

# Run as Root User
USER root

# Do Some Customization if Needed Here
RUN apk add --no-cache --update \
      inotify-tools \
    && mix archive.install hex phx_new ${PHOENIX_VERSION}}

# Run Command
CMD ["tail","-F","/dev/null"]
