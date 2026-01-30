FROM univer-acr-registry.cn-shenzhen.cr.aliyuncs.com/devops/debian:dev

ARG TARGETARCH

WORKDIR /app

RUN mkdir /app/web

COPY configs /app/configs
COPY bin/server-${TARGETARCH} /app/server
COPY web/public /app/web/public
COPY web/views /app/web/views

RUN chmod +x /app/server

CMD ["/app/server"]