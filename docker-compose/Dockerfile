FROM alpine:3.6

RUN \
  apk add --update git go make gcc musl-dev linux-headers && \
  git clone https://github.com/ethereum/go-ethereum       && \
  (cd go-ethereum && make geth)                           && \
  cp go-ethereum/build/bin/geth /usr/local/bin/           && \
  apk del git go make gcc musl-dev linux-headers          && \
  rm -rf /go-ethereum && rm -rf /var/cache/apk/*          && \
  echo 123




