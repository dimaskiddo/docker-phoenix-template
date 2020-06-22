FROM dimaskiddo/alpine:phoenix-1.5
MAINTAINER Team Name <team@mail.com>

# Run as Root User
USER root

# Do Some Customization if Needed Here
RUN apk add --no-cache --update --virtual .build-dep \
      build-base

# Run Command
CMD ["tail","-F","/dev/null"]
