FROM alpine
ADD test-ownership /usr/bin/
RUN adduser -D -H testuser && addgroup testgroup
RUN mkdir -p /vol/subvol
RUN chown testuser:testgroup /vol/subvol
VOLUME /vol/subvol
RUN touch /test
