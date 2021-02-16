FROM alpine:3.4


RUN apk --update add nodejs git openssh ca-certificates && \
    rm -rf /var/cache/apk/* && \
    npm install git2consul@0.12.13 --global && \
    mkdir -p /etc/git2consul.d
ADD gitconsul.json /etc/git2consul.d/gitconsul.json

ENTRYPOINT [ "/usr/bin/node", "/usr/lib/node_modules/git2consul" ]
