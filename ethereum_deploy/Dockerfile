FROM ubuntu:16.04
RUN apt-get update && apt-get install -y git && \
apt-get install -y curl && \
https://github.com/ethereum/go-ethereum && \
curl -sL https://deb.nodesource.com/setup_6.x | bash && \
apt-get install -y nodejs
EXPOSE 3200
ENTRYPOINT ["node","./TungServer/index.js"]
