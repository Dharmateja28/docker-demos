# Get basic image from docker hub and use this as base to build remaining.
FROM alpine

# install redis
RUN apk add --update redis

# default command to run once a a container starts from this image
CMD ["redis-server"]