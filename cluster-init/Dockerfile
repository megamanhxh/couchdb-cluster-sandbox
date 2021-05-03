FROM alpine:edge

RUN apk --no-cache add \
    curl \
    jq \
    dos2unix

COPY cluster-init.sh /cluster-init.sh

RUN dos2unix /cluster-init.sh

CMD [ "/cluster-init.sh" ]
